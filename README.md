# 🚀 Script de Criação de Estrutura de Diretórios e Usuários no Linux

Este projeto contém um script `bash` para automatizar a criação de diretórios, grupos de usuários, contas de usuário e configuração de permissões em um sistema Linux. Ideal para ambientes corporativos simulados, laboratórios de estudos e testes com gerenciamento de usuários.

---

## 📁 Estrutura Criada

O script cria os seguintes diretórios:

- `/publico` — Acesso total para todos os usuários.
- `/adm` — Exclusivo para o grupo `GRP_ADM`.
- `/ven` — Exclusivo para o grupo `GRP_VEN`.
- `/sec` — Exclusivo para o grupo `GRP_SEC`.

---

## 👥 Grupos Criados

- `GRP_ADM`
- `GRP_VEN`
- `GRP_SEC`

---

## 👤 Usuários Criados

| Nome        | Grupo     |
|-------------|-----------|
| carlos      | GRP_ADM   |
| maria       | GRP_ADM   |
| joao        | GRP_ADM   |
| debora      | GRP_VEN   |
| sebastiana  | GRP_VEN   |
| roberto     | GRP_VEN   |
| josefina    | GRP_SEC   |
| amanda      | GRP_SEC   |
| rogerio     | GRP_SEC   |

Todos os usuários recebem:

- Shell padrão `/bin/bash`
- Diretório home criado automaticamente
- Senha padrão `Senha123` (🚨 *recomenda-se trocar após o login inicial*)

---

## 🔒 Permissões de Acesso

| Diretório | Grupo      | Permissões |
|-----------|------------|------------|
| /publico  | Todos      | `rwxrwxrwx` (777) |
| /adm      | GRP_ADM    | `rwxrwx---` (770) |
| /ven      | GRP_VEN    | `rwxrwx---` (770) |
| /sec      | GRP_SEC    | `rwxrwx---` (770) |

---

## ⚙️ Como Executar<br>

1. Clone este repositório:<br>

- bash<br>
&nbsp;&nbsp;&nbsp;&nbsp;git clone https://github.com/GNunnes/linux-projeto1-iac.git<br><br>

2. Dê permissão de execução ao script:<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- bash<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;chmod +x script-criacao.sh<br>

3. Execute como root ou com sudo:<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- bash<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sudo ./script-criacao.sh<br>

🛡️ Requisitos <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Distribuição Linux (testado no Ubuntu Server 24.04)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Permissões de root<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Shell bash<br>

🧠 Conceitos Praticados <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Gerenciamento de usuários e grupos no Linux <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Permissões e propriedades de diretórios <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Scripts shell para automação de tarefas administrativas <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Princípios de segurança e organização de ambientes corporativos <br>

✍️ Autor<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;GNunnes<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;GitHub<br>

📜 Licença<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Este projeto está licenciado sob a MIT License.<br>

💡 Este script foi desenvolvido como parte de um projeto de Infraestrutura como Código (IaC) para fins educacionais.<br> 
Sinta-se à vontade para reutilizar e melhorar!<br>

yaml
---
Se quiser, posso gerar também o `LICENSE`, `.gitignore`, e criar um `Makefile` simples pra rodar o script com `make run`. Quer que eu inclua?








