# Android Crypto Monitor

Este projeto é um monitor de preços de criptomoedas utilizando a API do Mercado Bitcoin. Desenvolvido em **Kotlin** para Android, ele é dividido em 4 principais componentes:

## Estrutura dos Arquivos Kotlin

### 1. `MainActivity.kt`
Responsável pela **interface principal** do aplicativo.

- É a tela que o usuário vê.
- Faz a chamada para buscar os dados de preço utilizando o `MercadoBitcoinService`.
- Exibe o valor atual do Bitcoin no app.

**Resumo:** Ponto de entrada da aplicação e interface gráfica.

---

### 2. `TicketResponse.kt`
Representa o **modelo de dados**.

- Define a estrutura da resposta da API do Mercado Bitcoin.
- Contém propriedades como `high`, `low`, `last`, etc., que são os valores do mercado de cripto.

**Resumo:** Modelo que mapeia o JSON da resposta da API.

---

### 3. `MercadoBitcoinService.kt`
Define o **serviço de rede**.

- Interface que descreve como se comunicar com a API do Mercado Bitcoin usando Retrofit.
- Contém métodos HTTP (GET) para buscar informações sobre criptomoedas.

**Resumo:** Define como a aplicação se conecta à API.

---

### 4. `MercadoBitcoinServiceFactory.kt`
Cria instâncias do **serviço de rede**.

- Constrói o Retrofit configurado com a URL base da API.
- Fornece o `MercadoBitcoinService` pronto para ser usado na `MainActivity`.

**Resumo:** Fábrica para configurar o Retrofit e gerar o serviço da API.

**Evidência**

![image](https://github.com/user-attachments/assets/c3fdeb2c-fe56-4289-96cb-bd93ce1a76d0)


---

## Tecnologias Utilizadas
- **Kotlin**
- **Retrofit** (para comunicação HTTP)
- **Android Studio**

## Como rodar o projeto
1. Clone este repositório.
2. Abra no Android Studio.
3. Execute o projeto em um emulador ou dispositivo físico.

---


