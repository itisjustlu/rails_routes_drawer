# Rails routes drawer
This gem is intended to simplify your routes file. If you want to split it 
in multiples files to organize your routes, This is what you need.

### How to install?

```
gem 'rails_routes_drawer'
```

### How to use it?
Create a simple file under **config/routes/my_appended_routes.rb**

```
resources :products do
  resources :variants
end
```

and then in your config/routes.rb, just draw it!!

```
Rails.application.routes.draw do
  ...
  
  draw :my_appended_routes
  
  ...
end
```