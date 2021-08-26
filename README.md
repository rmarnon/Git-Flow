#Curso GitFlow

#1 - Inicializando o projeto:
#Git flow init -> Irá gerar as branches principais do projeto (Master e Developer).
#	Escolhe as nomenclaturas das ramificações de suporte (feature, bugfix, hotfix, release, support e prefixo de tag).
#*** Branches principais nunca serão apagadas, enquanto branches de suporte serão removidas após cada merge
#
#2 – Criando branch:
#Git flow feature start nomeDaBranch.
#*** Não é necessário colocar feature/, pois ele já cria automaticamente.
#	Desenvolve projeto normal, add, commit e da push normalmente.
#
#3 – Commitando na branch e finalizando:
#Git flow feature finish nomeDaBranch.
#*** dizendo que vou fechar a feature nomeDaBranch, e após operação, ele exclui a branch automaticamente

#4 - Criando release ao estar na Developer:
#Git flow release start 0.1.0 -> Representa o ambiente de Homologação
