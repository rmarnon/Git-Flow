Curso GitFlow

1 - Inicializando o projeto:
Git flow init -> Irá gerar as branches principais do projeto (Master e Developer).
	Escolhe as nomenclaturas das ramificações de suporte (feature, bugfix, hotfix, release, support e prefixo de tag).
*** Branches principais nunca serão apagadas, enquanto branches de suporte serão removidas após cada merge

2 – Criando branch:
Git flow feature start nomeDaBranch.
*** Não é necessário colocar feature/, pois ele já cria automaticamente.
	Desenvolve projeto normal, add, commit e da push normalmente.

3 – Commitando na branch e finalizando:
Git flow feature finish nomeDaBranch.
*** dizendo que vou fechar a feature nomeDaBranch, e após operação, ele exclui a branch automaticamente

4 - Criando release ao estar na Developer:
Git flow release start 0.1.0 -> Representa o ambiente de Homologação
*** Se tiver alteração na release, será atualizado tanto a developer, quanto a master automaticamente

5 - Criando merge da release para main:
Git flow release finish 0.1.0 -> Representa que sera mergeado para master
 *** Ele irá fazer o merge, e coloca :WQ! para confirmar, insere mensagem em seguida e :WQ para finalizar o merge. 
 
 6 - Criando hotfix é o mesmo processo, crado a partir da master:
 *** Se alterar a branch de hotfiz, irá atualizar tanto a master, quanto a developer
