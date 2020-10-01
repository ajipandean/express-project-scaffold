# Express Project Scaffold (EPS)
> Instant scaffold for structuring your Express project

Honestly, I want an instant project structure generator that suitable for my lovely current and future project.
That's why I created this repo :v so basically this is for my own sake

But if you want to use it as well, why not? There are steps you have to follow as shown bellow.

## Getting started
Before you start coding on your own, make sure you have forked and then clone this project.

```shell
// Using HTTPS
git clone https://github.com/YOUR_GITHUB_USERNAME/express-project-scaffold.git

// Using SSH
git clone git@github.com:YOUR_GITHUB_USERNAME/express-project-scaffold.git
```

Now, you have the structure on your computer. Next, let's install the dependencies to make this project works!

```shell
npm install
```

Okay, You almost finish. Last thing you have to do is to get your ```.env``` file.

```shell
cp .env.example .env
```

Great! Now, you're all set up. Let's start to make something awesome using Express!

## Structure
This structure follows MVC-style project you probably have seen in AdonisJS or Laravel for PHP.
Since we use Express as the core of this project, it is very flexible and customizable. Means that, you can add or remove almost everything if you need to.
> Get your freedom as developer by using Express

Below is the explanation of each folder in ```/src```. Again, you can add everything if you need to, or delete everything if you want to.

### config
This folder simply contains anything related to configuration. For example, want to make a connection to database? You can put your connection code here. 
Want to register all your environment variables? You can put your code here.

Or, Want to put your route handler here? Of course you can, but you waste the controllers folder at the end :v

### controllers
Well, this folder simply contains all your route handlers, but not included your CRUD logic, such as: fetch data from database or write data to database.
Those CRUD logic should be putted in folder called ```/services``` and ```/controllers``` contains all those code from ```/services```.

But, again, you can put everything here. Even your ```.gitignore``` file :v

### middlewares
Middleware is a set of code that executed before the request reaches route handlers.
So, if you have middleman to action, you put their code here. For example, you want to make authentication for protected routes? Put the code here.

### models
This folder contains codes where you want to specify the schema of your data.

### routes
Well, as the name it suggest. It contains all your routes. But, don't forget to import to your entry file, or it won't works.

### services
As I explain in ```/controllers``` folder. It contains all your CRUD related logic, such as insert data, fetch data, update data, and so on.

### util
Well, this folder maybe contains some of simple function that you want to import in several files.
I often use it to store my JSON Web Token Decoder code.

### validation
This folder contains all your validation for each request that would come to your route handlers.
Yeah, actually, this is middleware also. But putting all your validation related code in middleware folder looks messy for me. Then, I separated it.

Also, in some articles, I saw people put their validation code in separated folder. Cause that looks good to me, them I follow them.

## Closing
Okay! We are now at the end of README file :v again, this repo actually for my own sake. But, if you want to use it too, it's okay for me :v
Hmm... Yeah, if you have any opinion to improve this project structure, maybe you can pull request (?) :v
I'll be happy if you want to improve this project structure, so I can implement it in my currently working project or maybe future project :v

But, since this is public repo, other people who uses this project structure will be happy for the improvement, I guess :v

### Thank you & Happy coding!
