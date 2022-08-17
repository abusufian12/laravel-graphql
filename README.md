
php artisan lighthouse:ide-helper

composer require mll-lab/laravel-graphql-playground

php artisan thinker

php artisan vendor:publish --tag=lighthouse-config

php artisan route:list


----------------browse playground--------------------------
http://localhost:8000/graphql-playground

----------------Testing Example Code--------------------------
---------------
{
  user(id:2) {
    id,
    name,
    email
  }
}

----------------
{
  allusers {
    id,
    name,
    email
  }
}
----paginate-----------
{
  users(first:2, page:2) {
    data{
       id,
    	name,
    	email
    },
    	paginatorInfo{
        hasMorePages,
        currentPage,
        total
      }
  }
}
-----------------
mutation{
  createUser(
    name: "ssss",
    email: "ssss@gmail.com",
    password: "12345678"
  ){
    name
  }
}