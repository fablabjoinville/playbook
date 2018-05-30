# Inova Core i200

* [Descrição](#descrição)
* [Configuração dos Softwares](#tutorial-de-configurações-dos-softwares)
* [Funcionamento dos Softwares](#tutorial-de-funcionamento-dos-softwares)
* [Configuração da Impressora 3D](#tutorial-de-configuração-da-impressora-3d)
* [Problemas](#problemas)
* [Dicas](#dicas)

* [**Regras de Utilização**](https://github.com/fablabjoinville/playbook/blob/master/Regras-Fab-Lab.md)

## Descrição

Essa impressora 3D é da empresa [Inova 3D](https://www.inova3d.com.br/), de Biguaçu - SC.

Material online referente a ela, especificamente, é bem restrito.

Sua área de impressão é de 200mm (largura) X 200mm (profundidade) X 250mm (altura).

Para essa impressora, será usado o software [Repetier](https://www.repetier.com/) juntamente com o fatiador [Slic3r](http://slic3r.org/), o qual já acompanha o software. Opta-se por este pois permite uma configuração de impressão mais precisa e mais simples do que os demais.

Ela permite diversos tipo de materiais (filamentos), tais como PLA e ABS, pois dispõe de mesa aquecida e área de impressão isolada. **Atenção**: Nesse tutorial será passada a configuração para utilização do ABS, não usá-la com demais filamentos.

## Tutorial de Configuração dos Softwares

1. Download do [Repetier](https://www.repetier.com/);
2. Download da [configuração](https://github.com/fablabjoinville/playbook/tree/master/equipamentos/impressora-3d-inova-core-i200/slic3r-config-inova-core-i200.ini) de fatiamento no Slic3r;
3. Abrir Repetier e fazer a configuração da impressora, conforme imagens abaixo, na ordem de enumeração. Obs: abas sem foto não necessitam de alteração;

![Configuração da impressora no Repetier](https://github.com/fablabjoinville/playbook/tree/master/equipamentos/impressora-3d-inova-core-i200/repetier-config-inova-core-i200.png)

4. Importar configuração de fatiamento no Slic3r. Seguir imagens abaixo, na ordem de enumeração.

![Configuração de fatiamento no Slic3r](https://github.com/fablabjoinville/playbook/tree/master/equipamentos/impressora-3d-inova-core-i200/slic3r-config-inova-core-i200.png)

5. Pronto! Toda a configuração inicial está finalizada!

## Tutorial de Funcionamento dos Softwares

1. Abrir o molde para impressão no Repetier. Esse molde precisa estar na extensão .stl. Um site chamado [Thingiverse](https://www.thingiverse.com) dispõe de vários moldes, dá uma olhada lá!;

![Como abrir .stl no Repetier](https://github.com/fablabjoinville/playbook/tree/master/equipamentos/impressora-3d-inova-core-i200/repetier-open-stl-inova-core-i200)

2. Fatiar o molde usando o Slic3r, como mostrado abaixo. Obs: primeiro fazer o que está em vermelho;

![Como fatiar usando Slic3r](https://github.com/fablabjoinville/playbook/tree/master/equipamentos/impressora-3d-inova-core-i200/repetier-slice-slic3r-inova-core-i200)

3. Nesse momento o Slic3r deve abrir na sua tela. Clique em "Export G-code", abrirá o explorador de arquivos, não selecione outra pasta nem altere o nome do arquivo, apenas clique em "Salvar";

![Export G-code](https://github.com/fablabjoinville/playbook/tree/master/equipamentos/impressora-3d-inova-core-i200/slic3r-gcode-inova-core-i200)

4. No canto esquerdo inferior deve aparecer a mensagem "G-code file exported", após isso, feche o Sli3r, seu molde já estará fatiado no Repetier;
5. Agora basta salvar o arquivo gerado;

![Salvar Arquivo](https://github.com/fablabjoinville/playbook/tree/master/equipamentos/impressora-3d-inova-core-i200/repetier-save-inova-core-i200)

6. Esse arquivo salvo deve ser colocado no pen-drive que encaixará na impressora.
7. E é isto! Mais uma etapa finalizada. Bora configurar a impressora 3D agora.

## Tutorial de Configuração da Impressora 3D

1. Ligar a impressora 3D (botão na lateral direita);
2. Encaixar o pendrive, na lateral direita, com o arquivo g-code nele;
3. Abrir a portinha e abaixar o pino que fica no cabeçote, como na foto;

![Abaixar Cabeçote](https://github.com/fablabjoinville/playbook/tree/master/equipamentos/impressora-3d-inova-core-i200/cabecote-inova-core-i200)

4. Tirar todo resto de resíduo e plástico da mesa e limpar o bico de impressão, cortando o resto de filamento;
5. Na tela, clicar na engrenagem no canto direito inferior, depois no símbolo de fogo, no canto esquerdo inferior e em seguido, pressionar na frase "ABS";
6. Voltar para a tela inicial clicando no símbolo da porta, canto direito inferior;
7. Dos três quadrados clicáveis, pressionar o do meio e em seguida, dos novos três quadrados que aparecerá, clicar na opção pendrive da esquerda;
8. Pronto! Só aguardar a mesa e a extrusora aquecer que começará automaticamente a imprimir;

## Observações Extremamente Importantes

* Não manusear a impressora 3D sozinho se não estiver na [Lista](https://github.com/fablabjoinville/playbook/blob/master/Lista_Membros_Usar_Equipamentos.md) de pessoas autorizadas;
* Verificar atentamente a primeira camada que será impressa, em caso de alguma falha, apertar no quadrado do canto esquerdo inferior para cancelar a impressão imediatamente;
* Não abrir a portinha até o final da impressão, nem mudar as configurações da máquina;
* Ao finalizar a impressão, tirar o objeto e limpar a mesa, jogando no lixo adequado as sobras de filamento;
* Qualquer dúvida, perguntar para um guru.

## Problemas

Para resolver problemas na hora da impressão ou melhorar a impressão, a Simplify3D tem um guia muito completo [aqui](https://www.simplify3d.com/support/print-quality-troubleshooting/).

## Dicas

Dependendo do objeto impresso alguns detalhes precisam ser modificados, como por exemplo:

* **Layer Height** (grossura do plástico que sai)
* **Infill** (quanto mais % mais preenchimento)
* **Infill Pattern** (tipo de preenchimento)
* **Printing Temperature Initial Layer** (objeto não está grudando)
* **Generate Support** (necessita de suporte)
* **Build Plate Adhesion Type** (tipos de bases na impressão)

Para entender melhor, de uma olhada no guia da [Simplify3D](https://www.simplify3d.com/support/print-quality-troubleshooting/).