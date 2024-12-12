# DEIXAR-OS-BOT-ES-NA-HORIZONTAL-MOBILE

.buttons {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Layout flexível */
    gap: 20px;
    justify-content: center;
}



1. Usando flexbox

O Flexbox é uma abordagem muito comum para organizar itens na horizontal. Com essa técnica, você pode alinhar os botões de forma flexível.

.buttons {
    display: flex;
    justify-content: center; /* Alinha os botões no centro */
    gap: 20px; /* Espaçamento entre os botões */
}

.button {
    font-size: 1.5em;
    padding: 20px;
    background: linear-gradient(135deg, #6a0dad, #8a2be2, #4b0082);
    border: none;
    border-radius: 10px;
    color: white;
    cursor: pointer;
    transition: transform 0.3s ease;
    text-align: center;
}

display: flex;: Define o container como flexível, fazendo os itens (botões) se organizarem horizontalmente.

justify-content: center;: Alinha os itens ao centro do container.

gap: 20px;: Define o espaçamento entre os botões.


2. Usando inline-block

Você também pode usar inline-block para que os botões se comportem como elementos em linha, mas mantendo suas propriedades de bloco (como largura e altura).

.buttons {
    text-align: center; /* Centraliza os botões */
}

.button {
    display: inline-block; /* Deixa os botões em linha */
    font-size: 1.5em;
    padding: 20px;
    background: linear-gradient(135deg, #6a0dad, #8a2be2, #4b0082);
    border: none;
    border-radius: 10px;
    color: white;
    cursor: pointer;
    transition: transform 0.3s ease;
    text-align: center;
    margin: 10px; /* Espaçamento entre os botões */
}

display: inline-block;: Faz com que cada botão ocupe um espaço de bloco, mas se alinha horizontalmente como se fosse um elemento inline.

text-align: center;: Garante que os botões fiquem centralizados dentro do container pai.


3. Usando float

Embora não seja a técnica mais moderna, o float também pode ser usado para posicionar os botões horizontalmente.

.buttons {
    overflow: hidden; /* Para limpar o float */
}

.button {
    float: left; /* Faz com que os botões flutuem à esquerda */
    font-size: 1.5em;
    padding: 20px;
    background: linear-gradient(135deg, #6a0dad, #8a2be2, #4b0082);
    border: none;
    border-radius: 10px;
    color: white;
    cursor: pointer;
    transition: transform 0.3s ease;
    text-align: center;
    margin: 10px; /* Espaçamento entre os botões */
}

float: left;: Faz com que os botões flutuem para a esquerda, organizando-os horizontalmente.

overflow: hidden;: Usado no container para limpar o float, garantindo que o container envolva corretamente os elementos flutuantes.


4. Usando grid com diferentes configurações

Uma variação do layout grid pode ser feita usando grid-template-rows ou controlando o número de colunas de forma mais explícita.

.buttons {
    display: grid;
    grid-template-columns: repeat(6, 1fr); /* 6 colunas com igual largura */
    gap: 20px;
    justify-content: center;
}

.button {
    font-size: 1.5em;
    padding: 20px;
    background: linear-gradient(135deg, #6a0dad, #8a2be2, #4b0082);
    border: none;
    border-radius: 10px;
    color: white;
    cursor: pointer;
    transition: transform 0.3s ease;
    text-align: center;
}

grid-template-columns: repeat(6, 1fr);: Cria um grid com 6 colunas, todas com o mesmo tamanho.

gap: 20px;: Define o espaçamento entre os botões.


Essas são algumas das formas mais comuns de posicionar botões ou outros elementos horizontalmente usando CSS. Cada uma dessas abordagens tem suas particularidades, mas todas podem ser úteis dependendo do seu projeto.

