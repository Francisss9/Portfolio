<div align="center">

# Francisco Gomes

**Software para o setor automóvel, feito para funcionar onde o trabalho acontece.**

Estudante de Engenharia Informática no ISEP · Porto, Portugal

[![Kota](https://img.shields.io/github/v/release/Francisss9/Portfolio?filter=kota-v*&label=Kota%20vers%C3%A3o&color=ce0c24&style=for-the-badge)](https://github.com/Francisss9/Portfolio/releases?q=kota) [![Rasto](https://img.shields.io/github/v/release/Francisss9/Portfolio?filter=rasto-v*&label=Rasto%20vers%C3%A3o&color=3b3b3b&style=for-the-badge)](https://github.com/Francisss9/Portfolio/releases?q=rasto) [![TypeScript](https://img.shields.io/badge/TypeScript-strict-3178c6?style=for-the-badge&logo=typescript&logoColor=white)](#stack) [![Offline first](https://img.shields.io/badge/offline-first-2ea043?style=for-the-badge)](#kota)

[Kota](#kota) · [Rasto](#rasto) · [Como trabalho](#como-trabalho) · [Stack](#stack) · [Contacto](#contacto)

</div>

---

## Projetos

Oficinas e stands trabalham de luvas calçadas, com rede fraca e sem tempo para formulários. Construo ferramentas que abrem depressa, guardam tudo no dispositivo e produzem documentos prontos a entregar ao cliente.

| | Projeto | Para quem | Estado |
| :-: | --- | --- | --- |
| 🔧 | [**Kota**](#kota): orçamentos de reparação em PDF | Oficinas | Disponível em Android e Windows |
| 🚗 | [**Rasto**](#rasto): cada viatura, com tudo registado | Pequenos stands | Piloto online |

---

## Kota

> **Orçamentos de reparação para oficinas, no telemóvel e no computador, sem internet.**

O Kota cria orçamentos em PDF A4 com totais exatos, numeração sequencial e a marca da oficina. Os dados ficam cifrados no próprio dispositivo: sem conta, sem nuvem, sem anúncios.

<div align="center">

[![Descarregar](https://img.shields.io/badge/Descarregar-ultima%20vers%C3%A3o-ce0c24?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Francisss9/Portfolio/releases?q=kota) [![Site](https://img.shields.io/badge/Site-kota.francisgomesx.dev-111011?style=for-the-badge&logo=cloudflare&logoColor=white)](https://kota.francisgomesx.dev)

</div>

### O que faz

| | |
| --- | --- |
| **100% offline** | Funciona sem rede. Orçamentos e clientes nunca saem do dispositivo. |
| **PDF A4 profissional** | Cabeçalho com a marca da oficina, peças, mão de obra, IVA e total. |
| **Rápido no telemóvel** | Pensado para usar junto da viatura, com envio por WhatsApp em poucos toques. |
| **Dados cifrados** | SQLCipher com chave no Android Keystore; DPAPI no Windows; cópias `.kota` em AES-256-GCM. |
| **Android e Windows** | A mesma aplicação em todos os dispositivos. |
| **Licença anual** | MB WAY, Multibanco ou cartão. Sem renovação automática. |

### Engenharia

- **Aritmética financeira exata.** Montantes em cêntimos inteiros, quantidades em centésimos, percentagens em pontos-base, cálculos intermédios em `BigInt` com arredondamento *half-up*. Os totais são sempre derivados, nunca importados.
- **Camadas puras.** O domínio não conhece React, bases de dados nem PDF. Os efeitos secundários vivem isolados na infraestrutura.
- **Persistência transacional.** Contadores sequenciais atómicos e relógio de revisões (*CAS*) que impede sobrescrever versões mais recentes.
- **Privacidade por desenho.** Sem telemetria nem análise de tráfego. A única ligação à rede é o licenciamento, só após um clique explícito do utilizador, e nunca envia dados de clientes ou orçamentos.
- **Portão de qualidade antes de cada commit.** Testes unitários com cobertura de linhas ≥ 95%, build estrito, suite E2E em Playwright (390 px e 1440 px, teclado e movimento reduzido), verificação visual dos PDFs e auditoria de dependências.

```mermaid
flowchart LR
    P["presentation<br/>React"] --> A["application<br/>estado e filas"]
    A --> D["domain<br/>regras e Zod"]
    A --> I["infrastructure<br/>SQLite · Dexie · PDF"]
    I --> D
```

### Descarregar e instalar

Cada versão inclui o instalador para todos os dispositivos na [página de versões](https://github.com/Francisss9/Portfolio/releases?q=kota):

- **Android 10+:** `Kota-X.Y.Z.apk`. Descarregue, permita a instalação a partir de fontes desconhecidas quando o Android perguntar e toque em **Instalar**. Se já tem o Kota, instala-se por cima e os dados mantêm-se.
- **Windows (x64, portátil):** `Kota-X.Y.Z-x64.exe`. Sem instalação: guarde numa pasta e abra.

Cada versão traz um `SHA256SUMS` para confirmar a integridade do ficheiro. Para emitir PDF é necessária uma licença, ativada em **Definições → Licença**. Há uma experiência gratuita de 7 dias, por pedido.

---

## Rasto

> **Cada viatura, com tudo registado.**

Gestão para pequenos stands: viaturas, custos, pós-venda, importação de Excel e relatórios PDF com as secções que escolher. Funciona em modo local ou como piloto online.

<div align="center">

[![Abrir o piloto](https://img.shields.io/badge/Piloto-online-111011?style=for-the-badge&logo=cloudflare&logoColor=white)](https://rasto.fpsgomes9.workers.dev/) [![Versões](https://img.shields.io/badge/Rasto-vers%C3%B5es-ce0c24?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Francisss9/Portfolio/releases?q=rasto)

</div>

- **Ficha completa por viatura**, com custos e histórico de pós-venda.
- **Importação de Excel** para passar do ficheiro antigo ao sistema sem reescrever nada.
- **Relatórios PDF** com secções selecionáveis, prontos a partilhar.
- **Acesso controlado**: o piloto online só admite contas autorizadas pelo responsável do stand.

---

## Como trabalho

- **Primeiro o problema real.** Falo com quem usa a ferramenta e desenho à volta do dia a dia: uma mão ocupada, rede instável, o cliente à espera.
- **Dados do utilizador pertencem ao utilizador.** Offline por defeito, cifrado, sem contas desnecessárias.
- **Rigor onde o dinheiro passa.** Aritmética inteira, testes sobre cada regra de cálculo, PDFs verificados contra a especificação.
- **Documentar as decisões.** Arquitetura, segurança e design ficam escritos, para que o projeto continue a fazer sentido daqui a um ano.

---

## Stack

<div align="center">

![TypeScript](https://img.shields.io/badge/TypeScript-3178c6?style=flat-square&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/React-20232a?style=flat-square&logo=react&logoColor=61dafb) ![Vite](https://img.shields.io/badge/Vite-646cff?style=flat-square&logo=vite&logoColor=white) ![Tailwind](https://img.shields.io/badge/Tailwind-0f172a?style=flat-square&logo=tailwindcss&logoColor=38bdf8) ![Zod](https://img.shields.io/badge/Zod-3068b7?style=flat-square&logo=zod&logoColor=white) ![Capacitor](https://img.shields.io/badge/Capacitor-119eff?style=flat-square&logo=capacitor&logoColor=white) ![Electron](https://img.shields.io/badge/Electron-2b2e3a?style=flat-square&logo=electron&logoColor=9feaf9) ![SQLite](https://img.shields.io/badge/SQLite-003b57?style=flat-square&logo=sqlite&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-1c1c1c?style=flat-square&logo=supabase&logoColor=3ecf8e) ![Cloudflare](https://img.shields.io/badge/Cloudflare%20Workers-f38020?style=flat-square&logo=cloudflare&logoColor=white) ![Vitest](https://img.shields.io/badge/Vitest-6e9f18?style=flat-square&logo=vitest&logoColor=white) ![Playwright](https://img.shields.io/badge/Playwright-2ead33?style=flat-square&logo=playwright&logoColor=white)

</div>

---

## Contacto

Dúvidas, suporte ou pedido da aplicação: **[suporte@francisgomesx.dev](mailto:suporte@francisgomesx.dev)**

<div align="center">

<sub>Feito no Porto · Os instaladores e o `SHA256SUMS` de cada versão estão na <a href="https://github.com/Francisss9/Portfolio/releases">página de versões</a>.</sub>

</div>
