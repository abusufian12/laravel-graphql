
## url

http://localhost:8000/graphql-playground

## lighthouse website

https://lighthouse-php.com/6/getting-started/installation.html



## commands


## if new install

composer require nuwave/lighthouse

php artisan vendor:publish --tag=lighthouse-schema

composer require mll-lab/laravel-graphiql



## query example

##----------------------------------------

{
  allusers{
    id,
    name,
    email
  }
}

##----------------------------------------

{
  singleUser(id: 1){
    id,
    name,
    email
  }
}


##--------------------------------------------

{
  userByEmail(email: "katelyn.nienow@example.org"){
    id,
    name,
    email
  }
}


##---------------------

{
  users(first:2, page:2){
    name,
    email
  }
 
}
