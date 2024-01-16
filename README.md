# **Análise estatística sobre nascimento no Brasil 2000 - 2022 e a ocorrência de Sindrome de Down.**
​
O objetivo da análise é verificar referência nos dados que indiquem possíveis relações com a ocorrência de Sindrome de Down. O texto abaixo, extraído da internet, contém informações sobre a Sindrome de Down.
____________________________________________________________________________________________________________________________
​
## **Sindrome de Down**
​
Para entender melhor o termo vamos tentar explicar por partes começando pela origem do nome da síndrome.
Síndrome – Conjunto de características que prejudicam de algum modo o desenvolvimento do indivíduo.
​
Down – Sobrenome do médico que descreveu esta síndrome John Langdon Down .
​
A Síndrome de Down também pode ser chamada de trissomia do 21 e as pessoas que a possuem de trissômicos . Freqüentemente, a Síndrome de Down é chamada de "mongolismo" e as pessoas que a apresentam de "mongolóides". Todavia, estes termos são totalmente inadequados preconceituosos, criados a partir de descrições incorretas realizadas no passado e, por isso, devem ser evitados .
A síndrome de down é um atraso no desenvolvimento, das funções motoras do corpo e das funções mentais, o bebê é pouco ativo e “molinho” (hipotonia).
​
## **Causas**
​
Dentro de cada célula do nosso corpo, estão os cromossomos, responsáveis pela cor dos olhos, altura, sexo e também por todo o funcionamento e forma de cada órgão do corpo interno, como o coração, estômago, cérebro, etc. Cada uma das células possui 46 cromossomos, que são iguais, dois a dois, quer dizer, existem 23 pares ou duplas de cromossomos dentro de cada célula. Um desses cromossomos, chamado de nº21 é que está alterado na Síndrome de Down. A criança que possui a Síndrome de Down, tem um cromossomo 21 a mais, ou seja, ela tem três cromossomos 21 em todas as suas células, ao invés de ter dois. É a trissomia 21. Portanto a causa da Síndrome de Down é a trissomia do cromossomo 21. Podemos dizer que é um acidente genético. Esse erro não está no controle de ninguém.
​
​
**Fonte:** https://www.fiocruz.br/biosseguranca/Bis/infantil/sindrome-down.htm
​
____________________________________________________________________________________________________________________________
### **CID-10 Relacionados a Síndrome de Down**
 
- Q 90.0 - Síndrome de Down, trissomia do 21, por não disjunção meiótica
- Q 90.1 - Síndrome de Down, trissomia do 21, mosaicismo por não disjunção mitótica
- Q 90.2 - Síndrome de Down, trissomia 21, translocação
- Q 90.9 - Síndrome de Down, não específica
​
### **Fonte:** https://cid.ninsaude.com/, https://conclinica.com.br/
____________________________________________________________________________________________________________________________
​
# **Fonte dos dados da análise:**
​
#### **Dados públicos disponibilidazos pelo Governo do Brasil no Sistema de Informação sobre Nascidos Vivos – Sinasc**
​
O Sistema de Informações sobre Nascidos Vivos (Sinasc), foi implantado oficialmente a partir de 1990, com o objetivo de coletar dados sobre os nascimentos informados em todo território nacional e fornecer dados sobre natalidade para todos os níveis do Sistema de Saúde. 
​
A implantação do Sinasc ocorreu de forma gradual em todas as unidades da Federação e já vem apresentando em muitos municípios, desde o ano de 1994, um número maior de registros do que o publicado pelo IBGE com base nos dados de Cartório de Registro Civil.
​
O nascimento é um dos eventos vitais e seu monitoramento pode contribuir para o conhecimento da situação de saúde de uma população e a avaliação de políticas e ações de vigilância e atenção à saúde na área da saúde materno-infantil.
​
Descrição das informações: disponibilizada.
​
Os **registros são oriundos do sistema Sinasc**, contendo dados socioeconômicos, local de residência e ocorrência, anomalias congênitas, parto e pré natal.
​
Link para acesso aos dados: https://opendatasus.saude.gov.br/dataset/sistema-de-informacao-sobre-nascidos-vivos-sinasc
​
____________________________________________________________________________________________________________________________
​
# **Tratamentos Realizados nos Dados**
____________________________________________________________________________________________________________________________
​
### Ajustando a idade das mães em categoria e outros tratamentos
​
- Observação 1.
​
Verificou-se nos dados que existem 37.284 de registros ausentes na idada da mãe como também mães 835 com o registro de idade = 0.
​
Optou-se por remover esses dados uma vez que o objetivo e verificar relação entre a idade das mães e as ocorrências de Sindrome de Down.
​
- Observação 2.
​
Verificou-se tabém inconsistências nos dados referente a idade das mães: Há 1599 registro de idade da mãe na faixa entre 96-100 anos e que os demais dados se concentram entre as faixas 0-10 e 61-65 anos.
​
Esses dados também serão removidos.
____________________________________________________________________________________________________________________________
Referência para idade das mães:
​
"Uma mulher indiana pode ter se tornado a mãe mais velha do mundo ao **dar à luz aos 75 anos de idade**. Ela ficou grávida por meio de fertilização in vitro (FIV) e o bebê, uma menina, nasceu na noite do último sábado, 12, informou o The Times of India. No entanto, a médica que fez o parto não pode confirmar a idade da parturiente, uma vez que ela não levou documento de identidade"  
​
"**Mãe mais velha do mundo:** Um representante do **Guinness World Records disse ao Daily Mail que não havia evidência suficiente para atestar que Prabha é a mãe mais velha do mundo.** Para notificar um recorde, a equipe utiliza certidões de nascimento, censos e documentos hospitalares. Entrevistas com testemunhas independentes também são feitas para confirmar se a informação está correta. **De acordo com o Livro dos Recordes, Maria del Carmen Bousada Lara é a mãe mais velha do mundo. Ela deu à luz gêmeos, por cesárea, quando tinha 66 anos** e 358 dias de vida no hospital Sant Pau, em Barcelona, na Espanha, no dia 26 de dezembro de 2006." Por Ludimila Honorato em 15/10/2019. 
​
Fonte: https://www.estadao.com.br/emais/comportamento/mulher-pode-ser-a-mae-mais-velha-do-mundo-ao-dar-a-luz-aos-75-anos/
​
____________________________________________________________________________________________________________________________
​
### Ajustando a coluna Sexo
​
O valor 9 dessa coluna, não consta na documentação, presumido como Ignorado, conforme documentação da coluna gravidez
____________________________________________________________________________________________________________________________
​
### Ajustando a coluna Idanomal
​
O valor 8 e 5 dessa coluna, não consta na documentação, presumido como Ignorado, conforme documentação da coluna.
____________________________________________________________________________________________________________________________
​
### Ajustando a coluna QT_NASCIDOS
​
Foram removido registro nulos dos dados da quantidade de nascidos.
_____________________________________________________________________________________________________________________________

# Documentação da Tabela

Os dados passaram por uma limpeza na coluna idade mãe, removendo dados nulos ou com valores iguais a zero.

As Colunas possuem os seguintes dados:

| Nr | Coluna         | Descrição                                                                         |
|--------|--------------|------------------------------------------------------------------------------------|
| 0      | IDD_MAE      | Possui a informação da idade das mães.                                            |
| 1      | QT_NASCIDOS  | Possuem informações sobre o número de filhos gestados na gravidez.                |
| 2      | TIP_PARTO    | Apresenta informações do tipo de parto que foi realizado para o nascimento da criança. |
| 3      | SEXO         | Informa o sexo da criança.                                                        |
| 4      | PESO         | Informa o peso da criança ao nascer.                                              |
| 5      | IDFD_ANOMAL  | Informa se foi identificada alguma anomalia no nascimento da criança.             |
| 6      | CD_ANOMAL    | Consta a informação das anomalias identificadas nas crianças.                      |
| 7      | ANO          | Informa o ano de nascimento da criança.                                           |
| 8      | Q900         | Informa se o CID Q90.0 (Síndrome de Down, trissomia do 21, por não disjunção meiótica), foi identificada na criança. |
| 9      | Q901         | Informa se o CID Q90.1 (Síndrome de Down, trissomia do 21, mosaicismo por não disjunção mitótica), foi identificada na criança. |
| 10     | Q902         | Informa se o CID Q90.1 (Síndrome de Down, trissomia 21, translocação), foi identificada na criança. |
| 11     | Q909         | Informa se o CID Q90.9 (Síndrome de Down, não específica), foi identificada na criança. |
| 12     | QT_DOWN      | Informa a quantidade de anomalias relacionadas a Síndrome de Down foram identificadas. |
| 13     | IDFD_DOWN    | Identifica se a criação foi diagnosticada com Síndrome de Down.                   |
| 14     | FXA_IDD      | Mostra a idade das mães por categoria.                                           |
| 15     | TIP_GVD      | Informa o tipo de gravidez.                                                       |

