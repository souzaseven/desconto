# 🧮 Calculadora de Descontos
<!--
![Calculator Preview](https://github.com/souzaseven/horatrabalhada/blob/Desafios/Hora%20trabalhada/horatrabalhada.png?raw=true )
 Imagem com largura de 500px e altura proporcional -->
<img src="https://github.com/souzaseven/horatrabalhada/blob/Desafios/Hora%20trabalhada/horatrabalhada.png?raw=true" alt="Calculator Preview" width="500px" />
Uma calculadora interativa para calcular descontos em tempo real com exibição detalhada dos resultados.

## ✨ Funcionalidades

- **Cálculo Instantâneo**
  - Atualização automática ao digitar
  - Exibe valor original, porcentagem, valor final e diferença
  - Formatação monetária (R$)

- **Interface Intuitiva**
  - Design limpo e responsivo
  - Tabela organizada com resultados
  - Destaque visual nos valores importantes
  - Ícones do Font Awesome

- **Tecnologias Modernas**
  - HTML5 semântico
  - CSS3 com Flexbox e animações
  - JavaScript puro (ES6)

## 🎨 Design
```css
.container {
    background-color: #ffffff;
    border-radius: 15px;
    box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2);
    width: 450px;
}

.highlight {
    font-weight: bold;
    color: #007bff;
    background-color: #e0f0ff;
}
```
## ⚙️ Como Funciona
Lógica Principal
```javascript
function calcularDesconto() {
    const discountAmount = (originalPrice * discountPercentage) / 100;
    const finalPrice = originalPrice - discountAmount;
    
    finalValueTd.textContent = `R$ ${finalPrice.toFixed(2)}`;
    differenceValueTd.textContent = `R$ ${discountAmount.toFixed(2)}`;
}

Event Listeners
originalPriceInput.addEventListener('input', calcularDesconto);
discountPercentageInput.addEventListener('input', calcularDesconto);
```

##📊 Estrutura do Projeto

calculadora-descontos/ <br>
├── index.html          # Estrutura principal <br>
├── style.css           # Estilos modernos <br>
└── script.js           # Lógica de cálculo <br>


##📱 Responsividade
Layout centralizado verticalmente
Inputs com foco destacado
Tabela adaptável

```css
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
```
##🚀 Como Usar
Clone o repositório <br>
Abra index.html no navegador <br>

Insira: <br>
Valor original <br>
Porcentagem de desconto <br>
Veja os resultados atualizados automaticamente<br>

##📜 Licença
MIT License - Livre para uso e modificação
