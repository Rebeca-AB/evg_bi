# Projeto BI - Escola Virtual do Governo
## → Modelagem lógica dos dados  
A modelagem lógica foi desenvolvida utilizando a ferramenta **DrawDB** com a estrutura em esquema estrela (Star Schema).  

<img width="1089" height="679" alt="image" src="https://github.com/user-attachments/assets/ac3dd93b-2563-400d-9d9d-0443d5f97769" /><br>
* **Tabela Fato:**<br> 
  * `f_evg`: Reservados para dados sobre a matrícula (código, situação) e as chaves estrangeiras para a conexão com as tabelas dimensões.<br>
* **Tabelas Dimensão:**<br>
  * `dim_pessoa`: Reservados para dados sobre os estudantes (código, idade, e-mail, município, UF, esfera, etc.).<br>
  * `dim_turma`: Armazena os atributos específicos da turma (nome, modalidade, situação da turma).<br>
  * `dim_curso`: Detalha as características dos cursos (nome, carga horária, temática, conteúdo).<br>
* **Observações:**<br>
  * como a atividade era focado no esquema estrela dados como: esfera, poder, instituição, munícipio e uf que poderiam ser colocados em tabelas dimensões próprias em 'dim_poder' e 'dim_uf' e ligados para 'dim_pessoas' foram apenas inseridos em 'dim_pessoa' diretamente<br>
  
## → Dashboard<br>
<img width="1168" height="667" alt="image" src="https://github.com/user-attachments/assets/fd8341f6-324d-426d-9ed6-257aa4b72d5b" />
  
* **Perguntas:**<br>
  * `Total de alunos inscritos `: 188,11 mil<br>
  * `Curso maior quantidade de matrículas`: Boas Práticas de Manipulação em Serviços de Alimentação<br>
  * `Gênero com mais participação nos cursos`: Feminino com 100,81 mil - Masculino com 80,36 mil<br>
  * `Top 3 UF com mais alunos`: São Paulo (33,18 mil) - Rio de Janeiros (19,18 mil) - Minas Gerias (15,51 mil)<br> 
    
* **[ Exemplo de filtragem : ]**<br>
<img width="1168" height="663" alt="image" src="https://github.com/user-attachments/assets/01bafee2-bc9e-40f8-bf4b-3fe5bec84f56" /><br>
Data: inscritos dentro do período 2 meses (Maio - Junho)<br>
Curso: Comunicação assertiva<br>
UF: Na região do DF<br>
