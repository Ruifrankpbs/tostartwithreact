## Propriedades



# Imutabilidade
as propriedades sao somente leitura dentro do componente, ou seja, não podem ser alteradas diretamente;

# Padrões
Um componente pode definir valores default para as propriedades, caso nenhum seja fornecido;

# Composição
Elas pode ser usadas para renderizar outros componentes dentro do componente pai,tornando-o mais customizada.

# Children
é uma prop especial do React que representa o conteúdo passado entre as tags  do componente;

# Key
é uma prop usada pelo React para identificar elementos de uma lista e otimizar a renderização.

```
function Button ({children, variant }) {
    return (
        <button className={variant === 'primary' ? 'bg-purple-500' : 'bg-gray' }>
    )
    {children}
    </button>
}

function App() {
    return (
        <Button variant="prmary">Meu Botão</Button>
    )
}
```