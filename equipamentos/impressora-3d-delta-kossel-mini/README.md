
# Micromake Delta Kossel Mini

* [Descrição](#descricao)
* [Como usar](#como-usar)
* [Dicas](#dicas)
* [Problemas](#problemas)
* [Softwares](#softwares)
* [Configurações](#configuracoes)
* [Manutenção](#manutencao)
* [Referências](#referencias)

## Descrição

Essa impressora é baseada no kit de aprendizado da [Micromake](http://www.micromake.org/), uma empresa chinesa.

Para realizar pesquisas na internet, basta buscar pelos termos `Kossel Mini`, `Micromaker D1`, `MKS Mini`.

Nós estamos usando o *software* Cura para esta impressora. Você pode fazer o *download* da versão para Mac [aqui](https://drive.google.com/file/d/0B8ssrRNKTrw_SEViX2hucmZJNXM/view?usp=sharing) ou da versão Windowns [aqui](https://ultimaker.com/en/products/ultimaker-cura-software).

## Como usar

## Dicas

## Problemas

## Softwares

O Cura é um software com a funcionalidade de fatiar e configurar a impressão, não sendo usado para modelar o objeto. É necessário que o molde esteja na extensão .stl.

Antes de sair imprimindo é preciso configurar o Cura.

### Configuração

Seguir esses passos para configurar a impressora:

![Config_3D_Kossel-Mini](https://raw.githubusercontent.com/fablabjoinville/playbook/master/equipamentos/impressora-3d-delta-kossel-mini/Config_3D_Kossel-Mini.png)

Você pode baixar o [*profile* de configuração](https://raw.githubusercontent.com/fablabjoinville/playbook/master/equipamentos/impressora-3d-delta-kossel-mini/profile1.ini).

É necessário tomar alguns cuidados para não entupir o bico. Primeiro, comente ou apague o comando `M107` e adicione `M106 200` ou `255`:

![Cura 1](https://raw.githubusercontent.com/fablabjoinville/playbook/master/equipamentos/impressora-3d-delta-kossel-mini/cura-1.png)

Também mude o valor do *fan full on at height (mm)* para `0`:

![Cura 2](https://raw.githubusercontent.com/fablabjoinville/playbook/master/equipamentos/impressora-3d-delta-kossel-mini/cura-2.png)

## Configurações

## Manutenção

Neste diretório você encontra as peças que dão suporte do extrusor para impressão, nos formatos `stl` e `gcode`:

* hotend-clip
* suportebico

# Referências

* [Micromake](http://www.micromake.org/)
* [Repetier](https://www.repetier.com/)
* [How to start Micromake DIY Delta type 3D printer Auto calibration](https://www.youtube.com/watch?v=4H4AJsgLzyw)

