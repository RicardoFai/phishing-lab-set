# phishing-lab-set
# 🛡️ Laboratório Prático: Credential Harvesting com Social-Engineer Toolkit (SET)

## 📌 Descrição do Projeto
Este repositório documenta a execução de um laboratório prático de Engenharia Social focado na técnica de **Credential Harvesting** (captura de credenciais) utilizando a ferramenta **Social-Engineer Toolkit (SET)** em ambiente virtualizado controlado (Kali Linux).

O objetivo do exercício é demonstrar o funcionamento técnico de ataques de Phishing baseados em formulários web, analisando a mecânica de redirecionamento HTTP/POST e a importância de mecanismos de defesa como HTTPS estrito, HSTS e Autenticação Multifator (MFA).

> ⚠️ **Aviso de Isenção de Responsabilidade:** Este projeto foi executado estritamente para fins acadêmicos e educacionais em uma rede local privada (RFC 1918) isolada.

---

## 🧰 Ferramentas e Ambiente
* **Sistema Operacional:** Kali Linux (VM em modo Network Bridge)
* **Ferramenta Principal:** Social-Engineer Toolkit (`setoolkit`)
* **Endereço IP do Atacante (Local):** `192.168.2.120` (Porta HTTP 80)
* **Aplicação Alvo:** Web Template Interno (Google Login Page)

---

## ⚙️ Passo a Passo da Execução

### 1. Inicialização do SET
Início da ferramenta com privilégios de superusuário no terminal do Kali Linux:
```bash
sudo setoolkit
```
## 📸 Evidências do Laboratório

### Etapa 1: Configuração dos Menus e Escolha do Vetor
![Configuração Inicial no SET](Screenshot_2026-09-20_18_02_13.png)

### Etapa 2: Seleção do Web Template
![Seleção do Template Google](Screenshot_2026-09-20_18_02_25.png)

### Etapa 3: Inicialização do Servidor Web na Porta 80
![Servidor SET Ativo](Screenshot_2026-09-20_18_02_38.png)

### Etapa 4: Acesso à Página Falsa do Google no Navegador
![Página Cloned do Google](Screenshot_2026-09-20_18_02_50.png)

### Etapa 5: Inserção de Dados Fictícios de Teste
![Formulário Preenchido](Screenshot_2026-09-20_18_02_59.png)

### Etapa 6: Interceptação e Coleta de Credenciais via POST
![Credenciais Capturadas no Terminal](Screenshot_2026-09-20_18_04_04.png)
