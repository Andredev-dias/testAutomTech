![image](logo.png)

# Teste da Autom Tech aplicado através de uma tech recruiter, baseado nas tecnologias HTML e CSS.

# Executado por André Dias desenvolvedor Front End 🚀

<a id="Sumário"></a>

## Sumário

[HTML](#HTML)

[CSS](#CSS)

[ARQUITETURA](#ARQUITETURA)

**Ferramentas de Desenvolvimento**

![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)

**Aplicações**

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)

**DevOps**

![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

# Instruções de elaboraração do código CSS do teste 🎨

<a id="CSS"></a>

## CSS

- Configuração dos inputs foi otimizada ao máximo para nao se criar divs aleatórias e extra code.

-EX:

```css
input[type="range"] {
  width: 100%;
  height: 3px;
  background-color: #b7babc;
}

input[type="range"]::-webkit-slider-runnable-track {
  border: none;
  border-radius: 3px;
}

.range-wrap {
  width: auto;
  position: relative;
}
.range-value {
  position: absolute;
  top: 100%;
}
.range-value span {
  width: 80px;
  height: 24px;
  line-height: 24px;
  text-align: center;
  background: transparent;
  color: var(--inputInfo);
  font-size: var(--fontSizeInfos);
  display: block;
  position: absolute;
  left: 50%;
  transform: translate(-50%, 0);
  border-radius: 6px;
}

input[type="radio"] {
  width: 20px;
  height: 20px;
  background-color: #b7babc;
}
```

[⬆ Voltar ao Sumário](#Sumário)

# Instruções de elaboraração do código HTML do teste 📇

<a id="HTML"></a>

## HTML

- Código desenvolvido em inglês e palavras estáticas em português.

- Ordem estrutural da página: Procurando ser o mais semântico possível, dando classes css apenas para divs wrap e singularidades.

- Acabei usando algum javascript para demo e otimização da apresentação, apenas um bônus.

-EX:

```html
<div class="wrapLabelAndInput">
  <label for="velocity">Velocidade</label>
  <div class="range-wrap">
    <div class="range-value" id="rangeV"></div>
    <input
      id="range"
      type="range"
      min="0"
      max="120"
      value="50"
      step="1"
    />
  </div>
</div>
```

-EX:

```javascript
const range = document.getElementById("range"),
  rangeV = document.getElementById("rangeV");
setValue = () => {
  const newValue = Number(
      ((range.value - range.min) * 100) /
        (range.max - range.min)
    ),
    newPosition = 10 - newValue * 0.2;
  rangeV.innerHTML = `<span>${range.value} rpm</span>`;
  rangeV.style.left = `calc(${newValue}% + (${newPosition}px))`;
};
```

[⬆ Voltar ao Sumário](#Sumário)

# Elaboração da arquitetura de arquivos do projeto 📂

<a id="ARQUITETURA"></a>

## ARQUITETURA

- Muito simples contendo apenas uma pasta com arquivo HTML e outro CSS.
- Existe também um arquivo .png apenas para o README.md e o próprio, imagens não são usadas no projeto e importações ou links de ícones também não, por não haver necessidade.
- Foi utilizado uma google font linkada no head e setada no CSS.

[⬆ Voltar ao Sumário](#Sumário)

# Desenvolvedor </>

![YOUR github stats](https://github-readme-stats.vercel.app/api?username=Andredev-dias)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Andredev-dias)
