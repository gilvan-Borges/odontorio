# OdontoRio — Site Institucional de Clínica Odontológica

> **Projeto fictício desenvolvido para fins de estudo e prática de desenvolvimento web front-end.**

Site institucional responsivo fictício para a clínica **OdontoRio**. O projeto foi criado com o objetivo de praticar HTML, CSS, Bootstrap e JavaScript, simulando o site de uma clínica odontológica com páginas de apresentação de serviços e cadastro de clientes.

## Acesso ao projeto

[https://gilvan-borges.github.io/odontorio/](https://gilvan-borges.github.io/odontorio/)

---

## Funcionalidades

- Navbar responsiva com menu hamburguer (mobile)
- Modal de login com campos de acesso ao sistema
- Seção hero com chamada para agendamento de consulta
- Cards de serviços odontológicos com efeito hover em gradiente
- Carrossel de depoimentos de pacientes
- Seção de contato com endereço, horários e mapa integrado (Google Maps)
- Footer com links para redes sociais
- Página de cadastro de clientes com:
  - Máscaras de input (CPF, CEP, data)
  - Validação completa do formulário
  - Preenchimento automático de endereço via **ViaCEP API**

---

## Tecnologias Utilizadas

### Front-end

| Tecnologia | Descrição |
|---|---|
| **HTML5** | Estrutura semântica das páginas |
| **CSS3** | Estilização customizada com variáveis CSS e gradientes |
| **JavaScript** | Lógica de interação e consumo de API |

### Frameworks e Bibliotecas

| Biblioteca | Versão | Finalidade |
|---|---|---|
| **Bootstrap** | 5.x | Layout responsivo, grid, componentes (Navbar, Modal, Carousel) |
| **jQuery** | 3.7.1 | Manipulação do DOM e requisições AJAX |
| **jQuery Mask Plugin** | 1.14.16 | Máscaras de input (CPF `000.000.000-00`, CEP `00000-000`, data `00/00/0000`) |
| **jQuery Validate** | 1.21.0 | Validação de formulários com mensagens de erro em português |

### APIs Externas

| API | Finalidade |
|---|---|
| **ViaCEP** | Preenchimento automático de endereço a partir do CEP digitado |
| **Google Fonts** | Tipografia — família **Poppins** (pesos 400 e 600) |
| **Google Maps Embed** | Mapa interativo na seção de contato |

---

## Destaques Técnicos

- **Design Responsivo** — layout adaptável para mobile, tablet e desktop usando o sistema de grid do Bootstrap
- **CSS com variáveis** — paleta de cores centralizada via `--brand` e `--brand-dark` para fácil manutenção
- **Validação customizada** — regras de CPF brasileiro e data no formato BR implementadas via plugin `validateBR`
- **Consumo de API REST** — integração com ViaCEP usando `$.getJSON` para busca de endereço em tempo real
- **UX aprimorada** — foco automático no campo "Número" após o preenchimento do CEP

---

## Estrutura de Arquivos

```
odontorio/
├── index.html          # Página principal
├── cadastro.html       # Página de cadastro de clientes
├── css/
│   ├── bootstrap.min.css
│   └── styles.css      # Estilos customizados
├── js/
│   ├── bootstrap.bundle.min.js
│   └── validateBR.js   # Validações customizadas para CPF e data BR
└── img/
    └── ...             # Imagens e ícones SVG
```

---

## Como executar localmente

Basta abrir o arquivo `index.html` diretamente no navegador — não há dependência de build ou servidor.

```bash
# Ou utilize a extensão Live Server do VS Code para hot reload
```
