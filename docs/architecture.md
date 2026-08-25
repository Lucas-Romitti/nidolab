# Modelo de Dados — Nidolab

## Diagrama Entidade-Relacionamento

O Nidolab precisará armazenar os dados dos usuários, das equipes criadas e dos Pokémon que fazem parte de cada equipe.

Como um usuário pode criar várias equipes e uma equipe pode possuir vários Pokémon, será utilizada a entidade intermediária `EQUIPE_POKEMON` para representar a relação entre equipes e Pokémon.

```mermaid
erDiagram

    USUARIO ||--o{ EQUIPE : possui
    EQUIPE ||--o{ EQUIPE_POKEMON : contem
    POKEMON ||--o{ EQUIPE_POKEMON : participa

    USUARIO {
        string id PK
        string nome
        string email
        string senha
    }

    EQUIPE {
        string id PK
        string usuario_id FK
        string nome
        string geracao
        string estilo_jogo
    }

    POKEMON {
        string id PK
        int numero
        string nome
        string tipo_principal
        string tipo_secundario
        string imagem
    }

    EQUIPE_POKEMON {
        string id PK
        string equipe_id FK
        string pokemon_id FK
        int posicao
    }
```

### Entidades

**USUARIO:** armazena os dados necessários para identificação e login do usuário.

**EQUIPE:** armazena as equipes criadas pelos usuários, incluindo seu nome, geração e estilo de jogo.

**POKEMON:** representa os Pokémon disponíveis para serem adicionados às equipes. Seus dados poderão ser obtidos por meio de uma API pública.

**EQUIPE_POKEMON:** relaciona os Pokémon às equipes e registra a posição de cada Pokémon dentro da equipe.
