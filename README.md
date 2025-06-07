# Resumo e dicas da criação de uma instância SQL no Azure

 **Passo a Passo:**
 
1. Acesse o Portal Azure
URL: https://portal.azure.com

--Crie uma conta gratuita se ainda não tiver uma.

2. Crie um Recurso: SQL Database
Menu lateral: "Criar um recurso" > "Banco de Dados" > "Banco de dados SQL"

**-->Preencha:**

--Nome do banco

--Nome do servidor (crie um novo servidor se necessário)

--Região: Brasil Sul (se quiser menor latência)

--Autenticação: nome de usuário e senha

--Plano de preço: escolha o gratuito ou mais simples para testes

3. Configure o Servidor SQL
   
-->Configure o firewall para permitir conexões:

--Vá até "Servidores SQL" > seu servidor > "Configurações do firewall"

--Adicione seu IP local para liberar acesso

4. Conecte ao Banco via Azure Data Studio ou DBeaver
   
--Use as credenciais criadas

--String de conexão disponível no painel da instância no Azure

5. Teste com um Script SQL
   
--Crie uma tabela, insira dados e faça uma consulta para garantir que está funcionando

**DICAS**

+ A Azure faz backup automático, mas verifique a política de retenção.

+ Ative logs de diagnóstico se quiser acompanhar desempenho e erros.

+ Escolha uma região próxima a você (ex: Brazil South) para reduzir a latência.

+ Regiões próximas tendem a oferecer melhor desempenho.

+ Ao terminar o projeto/teste, exclua os recursos para evitar cobranças.


