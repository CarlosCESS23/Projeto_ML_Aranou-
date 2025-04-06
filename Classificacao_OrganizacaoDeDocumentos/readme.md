<h1> Classificação e organização de documentos</h1>


<h2> O que realmente deve-se fazer?</h2>

Classificar automaticamente o tipo de documento pelo candidato (Documentos de exemplo: RG, CPF, Histórico, certidão e etc)
E com isso organizar todo esses arquivos em pastas separadas (Ou seja, cada pasta, terá o nome do candidato) que serão nomeados pelo nome ( Também pode ser pelo CPF)

<h2> O que iremos utilizar?</h2>

<li>GitHub para repositório
<li>Jupyter-notebook 
<li> Python 3.10.16 com bibliotecas : Arquivos ( os, shutil, pathlib)
 e Machine Learning: ( Sklearning)


<h1> Como algoritmo deve-se funcionar?</h1>

Seguinte:

### Primeira Etapa: OCR

<li> <strong>O que a 1° equipe vai fazer:  </strong> A Primeira equipe que é responsável por isso, eles vão pegar os documentos que estarão formato de pdf ou jpg e vão utilizar <strong>OCR</strong> para "ler" o que está escrito nessas imagens</li>

<br>
<li><strong>Resultado:</strong> Depois da leitura, gera um arquivo de texto simples (Formato em txt), dentro desse arquivo, estarão as informações como ( <strong>CPF, RG, NOME e entre outros</strong> )

</li>

<h3> Segunda etapa: Análise e Validação das informações </h3>

<li> A nossa equipe, vai pegar esse arquivo (formato txt) gerado na 1° etapa, e com isso vamos utilizar
o Sklearn/Keras para vereficar se as informações estão lá e parecem está corretas, exemplos: 
</li>
<br>
<ol>
    <li>O CPF é válido? (Tem todos os digitos)</li>
    <li>O RG está presente?</li>
    <li> E outras informações que devem consta nesse pdf</li>
</ol>

E depois disso, o sistema vai dar uma "nota" para cada documento , dizendo qual a porcetangem de certeza que as inforamções estão corretas (Acima de 80% está ótimo)


<h3>Terceira Etapa: Organização dos Documentos(Criação de Pasta e manipulações de arquivos) </h3>

<li>Se realmente estiver tudo OK, vai ser criado nova pasta no computador para guardar os documentos desse candidato. o Nome da pasta vai ser número do CPF (Por conta de várias gentes com mesmo nome) 
</li>

<li> Depois de criar a pasta, iremos pegar o PDF original e tacar lá nessa pasta que acabou sendo criada, após isso apagamos o arquivo de texto temporario</li>

<h2>Divisão de Tarefa</h2>

<li> Dupla 1: (Adriano e o Kayo) : Cuida a parte da 3° etapa de Organização de Documento
</li> 
<li> Dupla 2: (Carlos e Mikael) : Cuida a parte da 2° Etapa de Análise e Validação das informações

