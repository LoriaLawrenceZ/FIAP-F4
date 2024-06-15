<div name="readme-top">
    <h1 align=center>CAPÍTULO 2</h1>
</div>

>**Capítulo 2 - Um Pouco Mais de Bootstrap**

# INTRODUÇÃO

Framework CSS para contrução do front-end de aplicações web e que utiliza um sistema de grid responsivo. Esse sistema permite desenvolver com grande facilidade páginas que se adaptam aos diferentes tamanhos de tela, como de smartphone, notebook etc.

Exemplo de código básico utilizando o Bootstrap:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap 5 Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container-fluid p-5 bg-primary text-white text-center">
  <h1>My First Bootstrap Page</h1>
  <p>Resize this responsive page to see the effect!</p> 
</div>
  
<div class="container mt-5">
  <div class="row">
    <div class="col-sm-4">
      <h3>Column 1</h3>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit...</p>
      <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris...</p>
    </div>
    <div class="col-sm-4">
      <h3>Column 2</h3>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit...</p>
      <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris...</p>
    </div>
    <div class="col-sm-4">
      <h3>Column 3</h3>        
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit...</p>
      <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris...</p>
    </div>
  </div>
</div>
</body>
</html>
```

Para desenvolver alguns exemplos, será utilizado o código que está disponível na **CDN** (*Content Delivery Network*), onde o jsDelivr fornece suporta à CDN para CSS e JavaScript do Bootstrap:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap 5 Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
```

<p align="right">(<a href="#readme-top">back to top</a>)

# FORMULÁRIOS

Os formulários são um meio muito utilizado de enviar informações, existem várias formas de disponibilizarmos os dados e os diferentes tipos de campos.

> Como Construir um Formulário e Utilizar Seus Componentes [[Formulário básico](Formulario/FormularioBasico.html)]

## Visão Geral

Os controles de formulário do Bootstrap melhoram os vários elementos existentes.

|                     **Elemento**                      | **Descrição**                                                                                                                                        |
|:-----------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------|
|                     `<fieldset>`                      | Não possuem bordas, preenchimentos ou margens para que possam ser facilmente usados como *wrappers* para entradas individuais ou grupos de entradas. |
|                      `<legend>`                       | Como *fieldsets*, também foram modificados para serem exibidos como um tipo de cabeçalho.                                                            |
|                       `<label>`                       | São definidos para **display: inline-block** permitir **margin** na aplicação.                                                                       |
| `<input>`<br>`<select>`<br>`<textarea>`<br>`<button>` | São endereçados principalmente por **Normalize**, mas **Reboot** remove seus **margin** e configurou os **line-height: inherit**                     |
|                     `<textarea>`                      | Foram modificados para serem redimensionáveis apenas verticalmente, pois o redimensionamento horizontal geralmente distorce o layout da página.      |
|                `<bottom>`<br>`<input>`                | Se tornaram elementos de botão e acrescentam o **cursor: pointer**                                                                                   |

Certifique-se de usar um atributo apropriado em todas as entradas (por exemplo, **email** para receber endereço de e-mail, ou **number** para informações numéricas) a fim de aproveitar os controles de entrada mais recentes, como verificação de e-mail, seleção de número e muito mais.

Exemplo básico de formulário:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Formulário Básico</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
  </head>
<body>
  <form>
    <div class="mb-3">
      <label for="idEmail" class="form-label">Email</label>
      <input type="email" class="form-control" id="idEmail" aria-describedby="emailHelp">
      <div id="emailHelp" class="form-text">Preencha corretamente o campo email</div>
    </div>
    <div class="mb-3">
      <label for="idPassword" class="form-label">Senha</label>
      <input type="password" class="form-control" id="idPassword">
    </div>
    <button type="submit" class="btn btn-primary">Enviar</button>
  </form>    
</body>
</html>
```

<p align="right">(<a href="#readme-top">back to top</a>)

# NOTAÇÃO