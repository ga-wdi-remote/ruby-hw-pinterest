# Pinspiration


- Create new rails app called `pinspiration_api`
- set up cors
- rails db:create
- models
  rails g model Board title
  rails g model Pin board:references title image_url
  rails db:migrate
  check schema
- seed
- controllers
  rails g controller boards
  rails g controller pins
- routes
    root to: "boards#index"
    resources :boards do
      resources :pins
    end
- test all your routes
