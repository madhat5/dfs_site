# dfs_site


- Update README --ox--
    - https://gist.github.com/madhat5

- App --x--
    - app setup (rails new name_app -d postgresql)
    - ensure dependencies (bundle install)
    - add gems (devise, pry-rails)

- User authentification --o--
    - Devise (rails g devise:install)
    - Update enviromnment (config/environments/development.rb)
    - Update application view (app/views/layouts/application.html.erb)
    - user model generate (rails g devise user >> rake db:create >> rake db:migrate)
    - update aplication (app/views/layouts/application.html.erb)
    - force not logged redirect (app/controllers/application_controller.rb)
    - copy all views to application (rails g devise:views)
    - update routes (config/routes.rb)

- Visual framework 
    - (skeleton, bootstrap, foundation, etc)

- Database --x-- 
    - database create/check (rake db:create >> rails dbconsole)
    - model create (rails g model Name >> rails g controller names)
        - x#tables
    - update migration files (db/migrate)
    - create JoinTable migrate (rails g migration CreateJoinTable table_names1 table_names2) …by alpha…
    - schema migrate/test (rake db:migrate / rails dbconsole)

- Test --ox--
    - launch server (rails s)
    - update README

- Models(Seeds) --ox--
    - models update (app/models/name.rb)
    - update seed.rb
    - import/test (rake db:seed / rails dbconsole)
    - model test (rails c >> Name.all)

- Routes --x--
    - route test (rake routes)
    - route create (config/route.rb => resources :names)

- Controller --o--
    - method writeup (per controller)
        - up to x7 (index, show, create, new, edit, update, delete)
            - user 
                - index (website landing) --x--
                - show (profile) --x--
            - note 
                - index (all notes page) --x--
                - show --x-- individual note page

- Views --o--
    - INDEX/SHOW/CREATE only to start
        - user index/show --x--
        - note index/show --o--
    - folder create (mkdir app/views/names)
    - views create (touch app/views/names/index.html.erb)
        - x5 (_form, show, new, edit)
    - visual framework updates

- Heroku
    - setup

- Test --ox--
    - launch server (rails s)
    - update README

- Extras
    - 
