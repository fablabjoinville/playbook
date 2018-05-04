
# Micromake Delta Kossel Mini

* [Descrição](#descrição)
* [Como usar](#como-usar)
* [Problemas](#problemas)
* [Softwares](#softwares)
* [Configurações](#configurações)
* [Manutenção](#manutenção)
* [Referências](#referências)

## Descrição

Essa impressora é baseada no kit de aprendizado da [Micromake](http://www.micromake.org/), uma empresa chinesa.

Para realizar pesquisas na internet, basta buscar pelos termos `Kossel Mini`, `Micromaker D1`, `MKS Mini`.

Nós estamos usando o *software* Cura para esta impressora. Você pode fazer o *download* da versão para Mac [aqui](https://drive.google.com/file/d/0B8ssrRNKTrw_SEViX2hucmZJNXM/view?usp=sharing) ou a versão para Windows e Linux [aqui](https://ultimaker.com/en/products/ultimaker-cura-software).

## Como usar

1. Abrir projeto no Cura (.stl)
2. Configurar a impressão
3. Fatiar (slice)
4. Salvar/Gerar .gcode no Cartão SD
5. Colocar na impressora
6. Selecionar o arquivo
7. Pronto :)

## Problemas

Para resolver problemas na hora da impressão ou melhorar a impressão, a Simplify3D tem um guia muito completo [aqui](https://www.simplify3d.com/support/print-quality-troubleshooting/).

## Softwares

Seguir todos os passos que estão com o quadriculado **vermelho** na imagem abaixo, na ordem enumerada.

**Quadrado Azul**: apagar o comando `M107` e adicionar `M106 200`.

![Config_3D_Kossel-Mini](https://raw.githubusercontent.com/fablabjoinville/playbook/master/equipamentos/impressora-3d-delta-kossel-mini/Config_3D_Kossel-Mini.png)

## Configurações

A imagem abaixo tem uma configuração comum para impressão:

![Configuração de Impressão](https://raw.githubusercontent.com/fablabjoinville/playbook/master/equipamentos/impressora-3d-delta-kossel-mini/Config_Impressao_3D_Kossel-Mini.png)

Entretanto, dependendo do objeto impresso alguns detalhes precisam ser modificados, como por exemplo:

* **Layer Height** (grossura do plástico que sai)
* **Infill** (quanto mais % mais preenchimento)
* **Infill Pattern** (tipo de preenchimento)
* **Printing Temperature Initial Layer** (objeto não está grudando)
* **Generate Support** (necessita de suporte)
* **Build Plate Adhesion Type** (tipos de bases na impressão)

Para entender melhor, de uma olhada no guia da [Simplify3D](https://www.simplify3d.com/support/print-quality-troubleshooting/).

## Manutenção

Neste diretório você encontra as peças que dão suporte do extrusor para impressão, nos formatos `stl` e `gcode`:

* hotend-clip
* suportebico

# Referências

* [Micromake](http://www.micromake.org/)
* [Repetier](https://www.repetier.com/)
* [How to start Micromake DIY Delta type 3D printer Auto calibration](https://www.youtube.com/watch?v=4H4AJsgLzyw)

