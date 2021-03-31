## Como adicionar os Botões da Esteira Digital em seu Site.

Veja abaixo os passos necessários para inserir os botões da Esteira Digital em seu site, e utilizar todos os recursos da nossa plataforma.

### 1º - Adicionar Biblioteca

Inserir entre as tags **HEAD** do site a chamada para o script da biblioteca da Esteira Digital

Exemplo:
```html {.line-numbers}
<script src="https://app.imoview.com.br/esteira/script.js" type="text/javascript"></script>
```

### 2º - Adicionar Botão (Agende sua Visita e Alugue Online)

Adicione o código abaixo no lugar onde você deseja que o botão seja mostrado. (Pode adicionar mais de um botão, duplicando o item abaixo e trocar apenas o Custom HTML colocando o texto desejado, exemplo: "Aluguel Online" e "Fazer proposta") </br>
<br/>**No lugar das variáveis substitua com os dados do imóvel que desejar.** 

**Obs:** o campo clienteConvenio é obtido no sistema Imoview, em "Detalhes convênio".

Exemplo:
```html {.line-numbers}
<script type="text/javascript">
    IMOVIEW.Exec({
        "htmlPersonalizado": '<button id="button-agenda-visita" class="btn btn-primary  btn-block" style="color: #fff;background-color: #ffffff;border-color: #ffffff;margin-top: 10px;">Agendar Visita</button>', //Opcional - caso queira personalizar o botão(recomendado).
        "textoBotaoOriginal": "", //Assume o texo a seguir como padrão se não html personalizado preenchido. - "Agende sua visita e alugue online"
        "clienteConvenio": "2", //Código convênio do cliente no Imoview.     
        "imovelId": "",
        "imovelUrlFotoPrincipal": "", //Informe a URL Absoluta da imagem (Ex: http://www.seudominio.com.br/imagem.jpg)
        "urlImovelnoSite": window.location.href,
        "imovelEndereco": "",
        "imovelNumero": "",
        "imovelComplemento": "",
        "imovelBairro": "",
        "imovelCidade": "",
        "imovelEstado": "",
        "imovelDormitorios": "",
        "imovelVagas": "",
        "imovelCep": "",
        "imovelValor": "", 
        "imovelCondominio": "",
        "imovelIptu": "",  
    });
</script>
```
