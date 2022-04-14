# sisEmprestimos
Um sisteminha para criar e gerenciar solicitações de crédito
Você irá precisar de PHP, Compose, Mysql para rodar esse sisteminha,
No caso do servidor eu estou utilizando Docker, a Imagem que utilizei está disponível no link abaixo, o mesmo tem um mini tutorial de como instalar o docker e o docker compose na tua máquina e como clonar a imagem do ambiente de desenvolvimento com o mysql, o apache e o PHP e gerar o container docker para começar a codar.
https://marcosteodoro.dev/blog/dockerizando-seu-ambiente-de-desenvolvimento-php/
Caso vocẽ não queira usar a mesma imagem docker que eu utilizei, as versões de cada componente estão listadas abaixo.
PHP versão 7.2, Apache 2 e o banco de dados MariaDB 10.3.
O script sql e o modelo Entidade Relacionamento do banco de dados está disponível no seguinte caminho app/Db.
O SGBD que usei foi o MYSQL WORKbench 8.0 64bits.

#Críticas

*Adicionaria um login para o cliente;
*Adicionaria um login para um administrador onde a função do mesmo seria monitorar e dar o aval final da contenplação ou não do Crédito solicitado;
*Adicionaria a integração com a Api do Serasa para análise de crédito automática.
Um exemplo seria o auxílio na tomada de decisão da concessão ou não do crédito solicitado, como nos exemplos listados abaixo.
Score >= 800 e Valor <= 5000 = Crédito Aprovado automaticamente,
Score >= 600 e < 800 = Análise do Administrador
Score < 600 = Crédito Negado
logicamente isso são exemplos pra ilustrar minha ideia, programando poderiámos criar regras muitos mais complexas e acertivas.
