# Projeto BI - Escola Virtual do Governo   
## → Modelagem lógica dos dados  
A modelagem lógica foi desenvolvida utilizando a ferramenta **DrawDB** com a estrutura em esquema estrela (Star Schema).  
<img width="908" height="569" alt="image" src="https://github.com/user-attachments/assets/f95e6af2-93af-4615-945a-6c2d7684bfb3" />   
* **Tabela Fato:**   
  * `f_evg`: Concentra os registros das matrículas, datas, situações e as chaves estrangeiras para conexão com as dimensões.   
* **Tabelas Dimensão:**   
  * `dim_pessoa`: Contém dados demográficos e institucionais do aluno/usuário (idade, e-mail, município, UF, esfera, etc.).   
  * `dim_turma`: Armazena os atributos específicos da turma (nome, modalidade, situação da turma).   
  * `dim_curso`: Detalha as características dos cursos (nome, carga horária, temática, conteúdo).   
