# Projeto-C-Imagens-Labirintos

Desenvolvimento de um programa em C que manipula imagens em tons de cinza vista como matriz de números inteiros de 1 byte. 
Funcionalidades: converte txt para imm(imagem em formato de matriz), thresholding, detecta componentes conexos, resolução de labirinto.

Para Executalo compilar immc.c juntamente com stack.c e matriz.c
$ gcc imm.c matriz.c stack.c -o imm

*imm -open file.txto ->  Abre uma imagem (formato texto) e mostra os valores dos pixels na tela
*imm -convert file.txt file.immo -> Converte uma imagem no formato file.txt para o formato file.imm 
*imm -open file.immo -> Abra uma imagem (formato binária) e mostra os valores dos pixels na tela
*imm -segment thr file.imm segfile.immo -> Faz o thresholding(limiarização da imagem) com um valor thr da imagem file.imm e escreve o resultado em segfile.imm
*imm -cc segfile.im outfileo -> Detecta os componentes conexos de uma imagem•imm -lab imlab.txt imlabout.txtoMostra o caminho a ser percorrido em um labirinto
