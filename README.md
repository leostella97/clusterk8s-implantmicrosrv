# Criação do Cluster Kubernetes e Implantação do Microservice-demo de Exemplo

<table>
	<ol>
		<li>Acesse o Console do GCP (https://console.cloud.google.com) e faça login na sua conta. Se você ainda não tiver uma conta, será necessário criar uma antes de prosseguir.</li>
		<li>Crie um novo projeto no GCP ou selecione um projeto existente onde deseja implantar o cluster Kubernetes. Um projeto no GCP serve como um espaço de trabalho isolado para seus recursos e serviços.</li>
		<li>No Console do GCP, no canto superior direito, clique no seletor de projetos e selecione o projeto no qual você deseja trabalhar.</li>
		<li>No menu de navegação do GCP, clique em "Kubernetes Engine" ou pesquise por "Kubernetes Engine" na barra de pesquisa. Isso levará você à página do Kubernetes Engine, onde você pode gerenciar seus clusters Kubernetes.</li>
		<li>Clique em "Criar cluster" para iniciar o processo de criação do cluster Kubernetes. Aqui, você terá a oportunidade de personalizar várias configurações do cluster, como nome, região/zona, tamanho e tipo das máquinas virtuais que serão usadas como nós do cluster, bem como outras configurações avançadas, se necessário. Também é possível habilitar recursos adicionais, como escalonamento automático e monitoramento.</li>
		<li>Após revisar e definir as configurações do cluster, clique em "Criar" para iniciar a criação do cluster Kubernetes. O GCP começará a provisionar os recursos necessários e configurar o ambiente do cluster. Isso pode levar alguns minutos para ser concluído.</li>
		<li>Uma vez que o cluster Kubernetes tenha sido criado com sucesso, você poderá implantar o microserviço de exemplo. Para isso, você precisará ter o arquivo de manifesto YAML do microserviço. Esse arquivo contém a definição do serviço, dos pods e de outros recursos necessários para executar o microserviço.</li>
		<li>No Console do GCP, abra o Cloud Shell clicando no ícone do terminal no canto superior direito da página. O Cloud Shell é um ambiente de linha de comando baseado na web que possui as ferramentas e as APIs necessárias para interagir com o GCP.</li>
		<li>No Cloud Shell, navegue até o diretório onde está localizado o arquivo de manifesto YAML do microserviço. Isso pode ser feito usando comandos como cd para navegar entre diretórios.</li>
		<li>Use o comando <code>kubectl</code> (a ferramenta de linha de comando do Kubernetes) para implantar o microserviço no cluster Kubernetes. Por exemplo, execute o seguinte comando:
<br><br>

			kubectl apply -f arquivo_manifesto.yaml

<p>Esse comando instrui o Kubernetes a criar os recursos especificados no arquivo de manifesto YAML. Isso inclui a criação dos pods, dos serviços e de outros objetos relacionados.</p>
	
<li>Após a implantação, você pode verificar o estado do seu microserviço usando o comando kubectl get pods para listar os pods em execução no cluster. Isso mostrará informações sobre os pods, como nome, status e endereço IP.</li>
</ol>
</table>
