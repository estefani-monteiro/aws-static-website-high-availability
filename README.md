# Hospedagem de Site Estático com Alta Disponibilidade na AWS

Projeto prático desenvolvido na AWS para implementar uma arquitetura de hospedagem de site estático utilizando Amazon S3, Amazon CloudFront e Origin Access Control (OAC), com foco em segurança, alta disponibilidade e desempenho.

---

## 📌 Visão Geral
* ☁️ Amazon S3 para armazenamento de arquivos estáticos
* 🌍 Amazon CloudFront para distribuição global de conteúdo (CDN)
* 🔒 Origin Access Control (OAC) para acesso seguro à origem
* 🛡️ Bucket privado, sem acesso público
* ⚡ Menor latência e melhor desempenho para os usuários

---

## 📖 Sobre o Projeto

Este laboratório demonstra a implementação de uma arquitetura para hospedagem de um site estático utilizando serviços nativos da AWS.

A solução foi construída com um bucket Amazon S3 privado e uma distribuição Amazon CloudFront protegida por Origin Access Control (OAC), garantindo que o conteúdo seja acessado de forma segura, sem exposição direta do bucket à internet.

Além de reforçar a segurança da infraestrutura, essa arquitetura proporciona distribuição global de conteúdo, menor latência e alta disponibilidade por meio da CDN da AWS.

---

## 🎯 Objetivos

* Hospedar um site estático utilizando o Amazon S3.
* Manter o bucket privado, sem acesso público.
* Distribuir o conteúdo utilizando o Amazon CloudFront.
* Configurar o Origin Access Control (OAC).
* Aplicar boas práticas de segurança, desempenho e alta disponibilidade.

---

## ☁️ Serviços AWS Utilizados

* Amazon S3
* Amazon CloudFront
* Origin Access Control (OAC)
* Bucket Policy

---

## 🚀 Etapas da Implementação

### 1. Configuração do Amazon S3

Foi criado um bucket Amazon S3 para armazenar os arquivos do site (HTML e demais recursos estáticos).

O bucket foi configurado como privado, impedindo o acesso direto aos arquivos pela internet. Dessa forma, todo o conteúdo é disponibilizado exclusivamente pelo Amazon CloudFront, reduzindo a superfície de exposição da aplicação e aumentando a segurança da arquitetura.

<img width="800" height="460" alt="image" src="https://github.com/user-attachments/assets/fa71cad0-1161-4d9a-b29b-c57cedf77856" />

---

### 2. Configuração do Amazon CloudFront e Origin Access Control (OAC)

Foi criada uma distribuição Amazon CloudFront para disponibilizar o conteúdo utilizando a infraestrutura global de Edge Locations da AWS.

Também foi configurado o Origin Access Control (OAC), permitindo que apenas o CloudFront possuísse permissão para acessar o bucket Amazon S3.

Essa abordagem elimina a necessidade de tornar o bucket público, fortalecendo a segurança da solução e seguindo as boas práticas recomendadas pela AWS para hospedagem de sites estáticos.

<img width="800" height="460" alt="image" src="https://github.com/user-attachments/assets/bde26d4f-3a26-43ba-834d-aaf4db29dedb" />


---

### 3. Validação da Solução

Após a implantação da infraestrutura, foi realizado o teste de acesso utilizando o domínio fornecido pelo Amazon CloudFront.

A validação confirmou que o conteúdo foi entregue corretamente pela CDN, mantendo o bucket Amazon S3 protegido contra acessos diretos e garantindo o funcionamento esperado da arquitetura.

<img width="800" height="505" alt="image" src="https://github.com/user-attachments/assets/9377d5a7-337d-43e5-b4fe-dcad8715e4c5" />


---

## ✅ Resultados Obtidos

* ✔ Bucket Amazon S3 protegido contra acesso público.
* ✔ Distribuição global de conteúdo utilizando Amazon CloudFront.
* ✔ Controle de acesso implementado com Origin Access Control (OAC).
* ✔ Entrega segura dos arquivos por meio da CDN da AWS.
* ✔ Arquitetura preparada para alta disponibilidade, segurança e melhor desempenho.

---

## 💡 Boas Práticas Aplicadas

* Bucket Amazon S3 configurado como privado.
* Restrição de acesso à origem utilizando Origin Access Control (OAC).
* Distribuição de conteúdo por CDN para redução da latência.
* Separação entre a camada de armazenamento (Amazon S3) e a camada de distribuição (Amazon CloudFront).
* Aplicação do princípio do menor privilégio para acesso ao bucket.

---

## 📚 Principais Aprendizados

Durante o desenvolvimento deste laboratório foi possível compreender, na prática:

* A diferença entre um bucket público e um bucket privado.
* O funcionamento do Amazon CloudFront como CDN.
* A importância do Origin Access Control (OAC) na proteção da origem dos dados.
* Como disponibilizar aplicações estáticas seguindo boas práticas de segurança na AWS.
* Os benefícios da distribuição global de conteúdo para redução de latência e melhoria da experiência do usuário.

---

## 🛠️ Tecnologias e Serviços

* AWS
* Amazon S3
* Amazon CloudFront
* Origin Access Control (OAC)
* Bucket Policy
* HTML

---


## 👩‍💻 Autora

**Estéfani Monteiro**

Cloud Computing | AWS | Infraestrutura em Nuvem | Cloud Security

🔗 LinkedIn: https://www.linkedin.com/in/estefanimonteiro

---

⭐ Se este projeto foi útil ou interessante para você, considere deixar uma estrela no repositório.

