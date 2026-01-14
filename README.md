# ABNT IQSC

## Informações gerais

Estilo de formatação de referências criado para se adequar ao formato numérico sobrescrito para elaboração de dissertações e teses do Instituto de Química de São Carlos da Universidade de São Paulo (IQSC/USP). 

O arquivo CSL foi desenvolvido de forma independente pelo autor. O Instituto de Química de São Carlos (IQSC/USP) não participou do seu desenvolvimento, não o endossa oficialmente e não se responsabiliza por eventuais erros, omissões ou divergências em relação às normas institucionais vigentes.

O arquivo foi desenvolvido para uso com o Mendeley Desktop versão 1.19.8 e o correspondente *plugin* no Microsoft Word. Não sei se funcionará corretamente com outros programas.

Adaptado de https://github.com/citation-style-language/styles/blob/master/associacao-brasileira-de-normas-tecnicas-numerico.csl

# O arquivo .csl

Arquivos CSL (Citation Style Language) são arquivos em formato XML que definem como citações e referências bibliográficas devem aparecer em um texto acadêmico. O único arquivo que você precisará baixar é o `ABNT_IQSC_numerado_2026.csl`.

Após baixar o arquivo, é preciso adicioná-lo ao Mendeley. Para isso, abra o Mendeley Desktop e acesse "View > Citation Styles > More Styles...". Depois, com a aba "Installed" selecionada,  arraste o arquivo `ABNT_IQSC_numerado_2026.csl` para a lista de estilos disponíveis. No campo "Citation and Bibliography Language" defina o idioma como "Portuguese (Brazil)" e clique em "Done". A opção já estará disponível no *plugin* do Word (pode ser necessário reiniciar o Word).

# Mendeley

O Mendeley Desktop é um software de gerenciamento de referências bibliográficas que permite organizar, armazenar e citar artigos científicos, livros e outros documentos acadêmicos.

O Mendeley apresenta diversas categorias de arquivos nas quais podemos salvar nossos documentos, porém, categorias diferentes possuem campos distintos, que nem sempre correspondem às informações requisitadas pela norma ABNT. Por isso, em alguns casos, precisamos salvar referências a certos documentos em formatos diferentes do óbvio. Mais explicações abaixo.

Para salvar referências no Mendeley sugiro usar arquivos `.ris` ou `.bib`, que contêm as informações em uma forma facilmente interpretada. Se você usar arquivos PDF diretamente, o Mendeley pode gerar referências erradas. Outra sugestão é salvar as referências com apenas a primeira letra capitalizada (além de nomes próprios, de espécies, etc.), pois é assim que elas são formatadas pela biblioteca.

# Tipos de referências formatadas corretamente pelo arquivo CSL

## Artigos científicos

Como salvar no Mendeley: Formato *Journal Article*. 

**Instruções**

Para que a cidade seja adicionada automaticamente à bibliografia, é preciso inserir manualmente essa informação no Mendeley, pois ela não é normalmente usada e não está presente nos arquivos `.ris` ou `.bib` que contêm as referências. Primeiro, é necessário habilitar o campo "City" nas entradas correspondentes a artigos. Para isso, acesse o menu "Tools" na barra superior e siga o caminho: "Tools > Options > Document details > Document type > Journal Article". Basta marca a opção "City" e esse campo passará a constar em todos os arquivos do tipo "Journal Article".

Em seguida, será necessário inserir a informação sobre a cidade em todas as referências correspondentes a artigos. Para encontrar essa informação, você pode acessar o site [abcdindex](https://abcdindex.com/) ou usar alguma das fontes recomendadas pela bilbioteca. Fiz um arquivo com algumas revistas e as cidades correspondentes, que disponibilizo no arquivo `journals-cities.txt`. É importante não incluir o país no campo "Country", caso contrário, ele será incluído junto com o nome da cidade. Uma dica para agilizar a adição da informação sobre as cidades é selecionar todas as referências correspondentes a uma mesma revista usando Shift+Click. Com isso, preenchendo o campo "City" apenas uma vez, todas as referências serão atualizadas.

ABNT: SOBRENOME, INICIAIS. Título. **Revista**, Volume, Número, Páginas, Ano.

Exemplo: YOUNG, S. S.; YUAN, F.; ZHU, M. Chemical descriptors are more important than learning algorithms for modelling. **Molecular Informatics**, v. 31, n. 10, p. 707–710, 2012. 

## Preprints

Como salvar no Mendeley: Formato *Web Page*.

**Instruções**

Adicione o campo "Genre" no Mendeley usando "Tools > Options > Document details > Document type > Web Page" e selecione "Genre". Preencha o campo Genre (por exemplo, escrevendo Preprint) de todas as referências que correspondem a *preprints*. SOMENTE os *preprints* poderão ter o campo "Genre" preenchido. O título do repositório (ex: arXiv, bioRxiv, ChemRxiv, etc.) deverá ser incluído no campo "Publication" e, se precisar citar um trabalho de algum repositório que não seja um desses três, será necessário incluir manualmente no arquivo `.csl`. Preencha os campos "Date Accessed" com a data de acesso e "URL" com o *link* para o *preprint*. Adicionalmente, o campo "Type of Work" não deve estar preenchido.

ABNT: SOBRENOME, INICIAIS. Título. **Repositório**, Ano. [Preprint]. Disponível em: URL completa. Acesso em: dia, mês abreviado. ano.

Exemplo: LUNDBERG, S. M.; LEE, S. I. A unified approach to interpreting model predictions. **arXiv**, 2017. [Preprint]. Disponível em: https://arxiv.org/abs/1705.07874. Acesso em: 21 abr. 2022.

## TCC, Dissertação, Tese

Como salvar no Mendeley: Formato *Thesis*. 

**Instruções**

No campo "Abstract", insira o tipo de trabalho, por exemplo: Tese (Doutorado em Química). No campo "University", insira a informação referente ao Departamento e a Universidade, separados por vírgula, por exemplo: Instituto de Química de São Carlos, Universidade de São Paulo. Não use o campo "Department" pois ele não é acessado pelo Word.

ABNT: SOBRENOME, INICIAIS. **Título**. Ano. Tipo – Universidade, Cidade, Ano.

Exemplo: BARNABE, R. F. **Análise do suprimento de frutas e sua sazonalidade**. 2011. Dissertação (Mestrado em Educação) – Escola de Engenharia de São Carlos, Universidade de São Paulo, São Carlos, 2011.

## Página da Web

Como salvar no Mendeley: Formato *Working Paper*.

**Instruções**

O Mendeley não é capaz de fornecer informações referentes a local e publicação para arquivos do tipo "Web Page". Para contornar, usamos o mesmo truque dos *preprints*: salvamos a referência no Mendeley como "Working Paper" e preenchemos o campo "Genre" com qualquer coisa (por exemplo, escreva webpage). Preencha o campo "Publisher" com o nome do site e o campo "City" com a cidade de publicação.

ABNT: SOBRENOME, INICIAIS. **Título da matéria**. Nome do Site, Local de publicação, Ano. Disponível em: URL completa. Acesso em: dia, mês abreviado. ano.

Exemplo (sem cidade): LANDRUM, G. **The RDKit Book**. RDKit, [s. l.], 2024. Disponível em: https://www.rdkit.org/docs/RDKit_Book.html. Acesso em: 19 fev. 2025.

Exemplo (com cidade): DRUGS FOR NEGLECTED DISEASES INITIATIVE. **Doença de Chagas: chegou o momento de acabar com 110 anos de invisibilidade**. DNDI, Genebra, 2019. Disponível em: https://www.dndial.org/2019/comunicacao-e-informacao/press-releases/doenca-de-chagas-chegou-o-momento-de-acabar-com-110-anos-de-invisibilidade/. Acesso em: 8 maio 2019.

## Programas de computador

Como salvar no Mendeley: Formato *Computer Program*. 

Instruções:

O Mendeley não exporta referências a "Computer Program" como deveria (software), mas sim como um arquivo genérico. Não encontrei uma forma de criar um estilo específico para esse caso, então deixei a formatação genérica no formato adequado para programas de computador.

ABNT: SOBRENOME, INICIAIS. **Título**. Versão. Local de publicação: Empresa, Ano.

Exemplo (sem local e empresa): LANDRUM, G. A. **RDKit: Open-source cheminformatics**. Versão: 2020_03_2. [s.l.], [s.n.], 2020.

Exemplo (com local e empresa): TICKLE, I. J.; FLENSBURG, C.; KELLER, P.; PACIOREK, W.; SHARFF, A.; VONRHEIN, C.; BRICOGNE, G. **STARANISO**. Cambridge, United Kingdom: Global Phasing Ltd., 2018.

## Outros formatos

Para outros tipos de documentos há uma formatação genérica, mas você também pode modificar o artigo `.csl`, ou modificar manualmente a referência genérica gerada.

## Sugestões e dúvidas

Usar a aba *Issues* do repositório.
