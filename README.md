<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=190&color=0:ce0c24,100:111011&text=Francisgomesx&fontColor=ffffff&fontSize=52&fontAlignY=38&desc=Software%20para%20o%20setor%20autom%C3%B3vel&descSize=20&descAlignY=60" alt="Francisgomesx: software para o setor automóvel" width="100%" />

<a href="https://github.com/Francisss9/Portfolio">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&pause=1800&color=CE0C24&center=true&vCenter=true&width=640&lines=Feito+para+funcionar+onde+o+trabalho+acontece;Estudante+de+Eng.+Inform%C3%A1tica+no+ISEP+%C2%B7+Porto" alt="Feito para funcionar onde o trabalho acontece" />
</a>

<br><br>

[![Kota](https://img.shields.io/github/v/release/Francisss9/Portfolio?filter=kota-v*&label=Kota%20vers%C3%A3o&color=ce0c24&style=for-the-badge)](https://github.com/Francisss9/Portfolio/releases?q=kota)
[![Rasto](https://img.shields.io/github/v/release/Francisss9/Portfolio?filter=rasto-v*&label=Rasto%20vers%C3%A3o&color=3b3b3b&style=for-the-badge)](https://github.com/Francisss9/Portfolio/releases?q=rasto)
[![TypeScript](https://img.shields.io/badge/TypeScript-strict-3178c6?style=for-the-badge&logo=typescript&logoColor=white)](#-stack)
[![Offline first](https://img.shields.io/badge/offline-first-2ea043?style=for-the-badge)](#-kota)

**[🔧 Kota](#-kota)** &nbsp;·&nbsp; **[🚗 Rasto](#-rasto)** &nbsp;·&nbsp; **[🧭 Como trabalho](#-como-trabalho)** &nbsp;·&nbsp; **[🛠️ Stack](#-stack)** &nbsp;·&nbsp; **[✉️ Contacto](#-contacto)**

</div>

<br>

## 🏁 Projetos

> [!NOTE]
> Oficinas e stands trabalham de luvas calçadas, com rede fraca e sem tempo para formulários. Construo ferramentas que **abrem depressa**, **guardam tudo no dispositivo** e **produzem documentos prontos a entregar ao cliente**.

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🔧 Kota</h3>
      <p><b>Orçamentos de reparação em PDF</b><br>para oficinas, sem internet.</p>
      <p>
        <img src="https://img.shields.io/badge/Android-3ddc84?style=flat-square&logo=android&logoColor=white" alt="Android" />
        <img src="https://img.shields.io/badge/Windows-0078d4?style=flat-square&logo=windows&logoColor=white" alt="Windows" />
        <img src="https://img.shields.io/badge/estado-dispon%C3%ADvel-2ea043?style=flat-square" alt="Disponível" />
      </p>
      <a href="#-kota"><b>Ver detalhes →</b></a>
    </td>
    <td width="50%" valign="top">
      <h3>🚗 Rasto</h3>
      <p><b>Cada viatura, com tudo registado</b><br>para pequenos stands.</p>
      <p>
        <img src="https://img.shields.io/badge/Web-111011?style=flat-square&logo=cloudflare&logoColor=white" alt="Web" />
        <img src="https://img.shields.io/badge/estado-piloto%20online-f59e0b?style=flat-square" alt="Piloto online" />
      </p>
      <a href="#-rasto"><b>Ver detalhes →</b></a>
    </td>
  </tr>
</table>

<br>

---

## 🔧 Kota

> ### Orçamentos de reparação para oficinas, no telemóvel e no computador, sem internet.

O Kota cria orçamentos em **PDF A4** com totais exatos, numeração sequencial e a marca da oficina. Os dados ficam **cifrados no próprio dispositivo**: sem conta, sem nuvem, sem anúncios.

<div align="center">

[![Descarregar](https://img.shields.io/badge/Descarregar-%C3%BAltima%20vers%C3%A3o-ce0c24?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Francisss9/Portfolio/releases?q=kota)
[![Site](https://img.shields.io/badge/Site-kota.francisgomesx.dev-111011?style=for-the-badge&logo=cloudflare&logoColor=white)](https://kota.francisgomesx.dev)

</div>

### ⚡ Do telemóvel ao cliente em poucos toques

```mermaid
flowchart LR
    A(["📱 Abrir o Kota"]) --> B["🧾 Novo orçamento"]
    B --> C["🔩 Peças e mão de obra"]
    C --> D["📄 PDF A4 com a marca da oficina"]
    D --> E(["💬 Enviar por WhatsApp"])

    classDef step fill:#111011,stroke:#ce0c24,color:#ffffff,stroke-width:2px
    classDef edge fill:#ce0c24,stroke:#ce0c24,color:#ffffff
    class B,C,D step
    class A,E edge
```

### ✨ O que faz

| | Funcionalidade | Detalhe |
| :-: | --- | --- |
| 📴 | **100% offline** | Funciona sem rede. Orçamentos e clientes nunca saem do dispositivo. |
| 📄 | **PDF A4 profissional** | Cabeçalho com a marca da oficina, peças, mão de obra, IVA e total. |
| 📱 | **Rápido no telemóvel** | Pensado para usar junto da viatura, com envio por WhatsApp em poucos toques. |
| 🔐 | **Dados cifrados** | SQLCipher com chave no Android Keystore; DPAPI no Windows; cópias `.kota` em AES-256-GCM. |
| 🖥️ | **Android e Windows** | A mesma aplicação em todos os dispositivos. |
| 🎟️ | **Licença anual** | MB WAY, Multibanco ou cartão. Sem renovação automática. |

### 📊 Em números

<div align="center">

| 🧪 Cobertura de testes | 📐 Viewports testados | 🔒 Cifra das cópias | 🎁 Experiência gratuita |
| :-: | :-: | :-: | :-: |
| **≥ 95%** de linhas | **390 px** e **1440 px** | **AES-256-GCM** | **7 dias**, por pedido |

</div>

### 🧱 Engenharia

<details open>
<summary><b>Aritmética financeira exata</b></summary>

<br>

Montantes em **cêntimos inteiros**, quantidades em centésimos, percentagens em pontos-base, cálculos intermédios em `BigInt` com arredondamento *half-up*. Os totais são sempre **derivados**, nunca importados.

</details>

<details>
<summary><b>Camadas puras</b></summary>

<br>

O domínio não conhece React, bases de dados nem PDF. Os efeitos secundários vivem isolados na infraestrutura.

```mermaid
flowchart LR
    P["presentation<br/>React"] --> A["application<br/>estado e filas"]
    A --> D["domain<br/>regras e Zod"]
    A --> I["infrastructure<br/>SQLite · Dexie · PDF"]
    I --> D

    classDef core fill:#ce0c24,stroke:#ce0c24,color:#ffffff
    classDef layer fill:#111011,stroke:#ce0c24,color:#ffffff,stroke-width:2px
    class D core
    class P,A,I layer
```

</details>

<details>
<summary><b>Persistência transacional</b></summary>

<br>

Contadores sequenciais atómicos e relógio de revisões (*CAS*) que impede sobrescrever versões mais recentes.

</details>

<details>
<summary><b>Privacidade por desenho</b></summary>

<br>

Sem telemetria nem análise de tráfego. A única ligação à rede é o licenciamento, só após um clique explícito do utilizador, e **nunca** envia dados de clientes ou orçamentos.

</details>

<details>
<summary><b>Portão de qualidade antes de cada commit</b></summary>

<br>

- [x] Testes unitários com cobertura de linhas ≥ 95%
- [x] Build estrito
- [x] Suite E2E em Playwright (390 px e 1440 px, teclado e movimento reduzido)
- [x] Verificação visual dos PDFs
- [x] Auditoria de dependências

</details>

### 📥 Descarregar e instalar

Cada versão inclui o instalador para todos os dispositivos na [**página de versões**](https://github.com/Francisss9/Portfolio/releases?q=kota).

| | Plataforma | Ficheiro | Como instalar |
| :-: | --- | --- | --- |
| 🤖 | **Android 10+** | `Kota-X.Y.Z.apk` | Descarregue, permita fontes desconhecidas quando o Android perguntar e toque em **Instalar**. Se já tem o Kota, instala-se por cima e os dados mantêm-se. |
| 🪟 | **Windows (x64, portátil)** | `Kota-X.Y.Z-x64.exe` | Sem instalação: guarde numa pasta e abra. |

> [!TIP]
> Cada versão traz um `SHA256SUMS` para confirmar a integridade do ficheiro.

> [!IMPORTANT]
> Para emitir PDF é necessária uma licença, ativada em **Definições → Licença**. Há uma experiência gratuita de 7 dias, por pedido.

<br>

---

## 🚗 Rasto

> ### Cada viatura, com tudo registado.

Gestão para pequenos stands: viaturas, custos, pós-venda, importação de Excel e relatórios PDF com as secções que escolher. Funciona em **modo local** ou como **piloto online**.

<div align="center">

[![Abrir o Rasto](https://img.shields.io/badge/Abrir-rasto.francisgomesx.dev-111011?style=for-the-badge&logo=cloudflare&logoColor=white)](https://rasto.francisgomesx.dev)
[![Versões](https://img.shields.io/badge/Rasto-vers%C3%B5es-ce0c24?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Francisss9/Portfolio/releases?q=rasto)

</div>

### 🔄 Do Excel ao relatório

```mermaid
flowchart LR
    X(["📊 Excel antigo"]) --> I["📥 Importação"]
    I --> F["🚗 Ficha da viatura<br/>custos e pós-venda"]
    F --> R(["📄 Relatório PDF<br/>secções à escolha"])

    classDef step fill:#111011,stroke:#ce0c24,color:#ffffff,stroke-width:2px
    classDef edge fill:#ce0c24,stroke:#ce0c24,color:#ffffff
    class I,F step
    class X,R edge
```

### ✨ O que faz

| | Funcionalidade | Detalhe |
| :-: | --- | --- |
| 🗂️ | **Ficha completa por viatura** | Com custos e histórico de pós-venda. |
| 📥 | **Importação de Excel** | Passe do ficheiro antigo ao sistema sem reescrever nada. |
| 📄 | **Relatórios PDF** | Secções selecionáveis, prontos a partilhar. |
| 🔑 | **Acesso controlado** | O piloto online só admite contas autorizadas pelo responsável do stand. |

<br>

---

## 🧭 Como trabalho

| | Princípio | Na prática |
| :-: | --- | --- |
| 🎯 | **Primeiro o problema real** | Falo com quem usa a ferramenta e desenho à volta do dia a dia: uma mão ocupada, rede instável, o cliente à espera. |
| 🛡️ | **Os dados são do utilizador** | Offline por defeito, cifrado, sem contas desnecessárias. |
| 🧮 | **Rigor onde o dinheiro passa** | Aritmética inteira, testes sobre cada regra de cálculo, PDFs verificados contra a especificação. |
| 📝 | **Documentar as decisões** | Arquitetura, segurança e design ficam escritos, para que o projeto continue a fazer sentido daqui a um ano. |

<br>

---

## 🛠️ Stack

<div align="center">

**Aplicação**<br>
![TypeScript](https://img.shields.io/badge/TypeScript-3178c6?style=for-the-badge&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/React-20232a?style=for-the-badge&logo=react&logoColor=61dafb) ![Vite](https://img.shields.io/badge/Vite-646cff?style=for-the-badge&logo=vite&logoColor=white) ![Tailwind](https://img.shields.io/badge/Tailwind-0f172a?style=for-the-badge&logo=tailwindcss&logoColor=38bdf8) ![Zod](https://img.shields.io/badge/Zod-3068b7?style=for-the-badge&logo=zod&logoColor=white)

**Plataformas**<br>
![Capacitor](https://img.shields.io/badge/Capacitor-119eff?style=for-the-badge&logo=capacitor&logoColor=white) ![Electron](https://img.shields.io/badge/Electron-2b2e3a?style=for-the-badge&logo=electron&logoColor=9feaf9)

**Dados e cloud**<br>
![SQLite](https://img.shields.io/badge/SQLite-003b57?style=for-the-badge&logo=sqlite&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-1c1c1c?style=for-the-badge&logo=supabase&logoColor=3ecf8e) ![Cloudflare](https://img.shields.io/badge/Cloudflare%20Workers-f38020?style=for-the-badge&logo=cloudflare&logoColor=white)

**Qualidade**<br>
![Vitest](https://img.shields.io/badge/Vitest-6e9f18?style=for-the-badge&logo=vitest&logoColor=white) ![Playwright](https://img.shields.io/badge/Playwright-2ead33?style=for-the-badge&logo=playwright&logoColor=white)

</div>

<br>

---

## ✉️ Contacto

<div align="center">

Dúvidas, suporte ou pedido da aplicação:

[![Email](https://img.shields.io/badge/suporte%40francisgomesx.dev-ce0c24?style=for-the-badge&logo=gmail&logoColor=white)](mailto:suporte@francisgomesx.dev)

<br>

<sub>Feito no Porto 🇵🇹 · Os instaladores e o `SHA256SUMS` de cada versão estão na <a href="https://github.com/Francisss9/Portfolio/releases">página de versões</a>.</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&height=100&color=0:111011,100:ce0c24&section=footer" alt="" width="100%" />

</div>
