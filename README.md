
# Formulário de Matrícula - Rocket Seat

Uma página inicial para um formulário para matrícula na escola "Estrelas do Amanhã" com cadastro nome, data, email, telefone, envio de arquivos e mais.

## Sumário:
- [Geral](#geral)
  - [Screenshot](#screenshot)
  - [Links](#-links)
- [Processo de criação](#processo-de-craicao)
  - [Feito com:](#feito-com)
  - [Aprendizado](#aprendizado)
- [Autor](#autor)

## Geral

### Screenshot

![Final Project](final-project-screenshot.png)

### 🔗 Links

- Solution URL: [https://github.com/FYLIPI-2004/Formulario-de-Matricula](https://github.com/FYLIPI-2004/Formulario-de-Matricula)
- Live Site URL: [https://fylipi-2004.github.io/Formulario-de-Matricula/](https://fylipi-2004.github.io/Formulario-de-Matricula/)

## Processo de criação

### Feito com:

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Nesting CSS
- Form:
  - Input text
  - Input number
  - Input email
  - Input tel
- Fieldset

### Aprendizado

`inputs` em geral:
```
            <div class="input-wrapper">
              <label for="birth">Data de nascimento</label>
              <input type="date" id="birth" name="birth" lang="pt-BR">
            </div>

            <div class="select-wrapper">
              <label for="gender">Sexo</label>
              <select name="gender" id="gender">
                <option value="female">Feminino</option>
                <option value="male">Masculino</option>
                <option value="na">Prefiro não responder</option>
              </select>
            </div>
```
Aplicação do `fieldset`:

```
<fieldset class="address">
            <legend>Endereço residencial</legend>

            <div class="input-wrapper">
              <label for="">CEP</label>
              <input type="text" id="cep" name="cep">
            </div>

            <div class="flex">
              <div class="input-wrapper flex-2">
                <label for="street">Rua</label>
                <input type="text" id="street" name="street" value="Rua das Flores" disabled>
              </div>

              <div class="input-wrapper flex-1">
                <label for="number">Número</label>
                <input type="number" id="number" name="number">
              </div>
            </div>

            <div class="flex">
              <div class="input-wrapper flex-2">
                <label for="city">Cidade</label>
                <input type="text" id="city" name="city" value="São Paulo" disabled>
              </div>

              <div class="input-wrapper flex-1">
                <label for="state">Estado</label>
                <input type="text" id="state" name="state" disabled value="SP">
          </fieldset>
```

Utilização do Nesting CSS:
```
  .checkbox-image {
    flex: 0 0 1.5rem;
    height: 1.5rem;

    background-image: url(../../assets/icons/checkbox-default.svg);
  }

  &:hover, &:focus-within {
    .checkbox-image {
      background-image: url(../../assets/icons/checkbox-hover.svg);
    }
  }

  &:has(:checked) .checkbox-image {
    background-image: url(../../assets/icons/checkbox-checked.svg);
  }
  
}
```

## Autor

- [@FYLIPI-2004](https://github.com/FYLIPI-2004)
