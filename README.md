============================
        NOTES APP
============================

Aplicacao de anotacoes desenvolvida com Laravel (PHP),
simulando um servico completo de criacao e gerenciamento de notas.


==============================
  COMO RODAR O PROJETO
==============================

1. Instale as dependencias:
   composer install

2. Configure o ambiente:
   - Copie o arquivo .env.example e renomeie para .env
   - Ajuste as variaveis de ambiente conforme necessario

3. Gere a chave da aplicacao:
   php artisan key:generate

4. Crie e popule o banco de dados:
   php artisan migrate
   php artisan db:seed

5. Faca o cache dos icones (obrigatorio):
   php artisan icons:cache

6. Rode a aplicacao:
   php artisan serve


==============================
  COMANDOS UTEIS
==============================

php artisan optimize      -> Otimiza a aplicacao (opcional)
php artisan icons:clear   -> Limpa o cache dos icones
php artisan icons:cache   -> Refaz o cache dos icones


==============================
  OBSERVACAO
==============================

Sempre que adicionar novos icones na aplicacao,
rode os seguintes comandos na ordem:

   php artisan icons:clear
   php artisan icons:cache
