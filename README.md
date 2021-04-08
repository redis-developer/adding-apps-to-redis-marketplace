To add your project to Redis Marketplace:
1. Add the following `marketplace.json` file to your repository's root. 
2. Open an issue on this project asking for us to fork it.
3. Make sure the "hidden" flag is `true`. We'll switch it to `false` after we review it and fork it. 
4. Your app will be live automatically.


Modify the following `marketplace.json`. The details for each property are provided in comments.
```
{
    "app_name": "Basic Redis caching example in Nodejs",  //Name of the app
    "description": "Showcases how to impliment caching in NodeJS", // One line description
    "hidden": false, // Can be "true" or "false". If true, this app won't show up in Marketplace.
    "rank": 20, // This is used to sort the apps in the marketplace. 1 to 20 are reserved. Enter greater than 20
    "type": "Building Block", //Can be "Building Block" or "Full App"
    "contributed_by": "Redis Labs", // Can be "Redis Labs" or "Community" or "Partner"
    "repo_url": "https://github.com/redis-developer/basic-caching-demo-nodejs", //This is the Gitub Repo's URL.
    "download_url": "https://github.com/redis-developer/basic-caching-demo-nodejs/archive/main.zip",
    "hosted_url": "", //The URL of the app. if you are hosting this app somewhere
    "quick_deploy": "true", //"frue" if the project has Heroku, Vercel, Google deploy buttons
    "deploy_buttons": [
        {
            "heroku": "https://heroku.com/deploy?template=https://github.com/redis-developer/basic-caching-demo-nodejs" //Deploy button URL for deploying on Heroku
        },
        {
            "vercel": "https://vercel.com/new/git/external?repository-url=https%3A%2F%2Fgithub.com%2Fredis-developer%2Fbasic-caching-demo-nodejs&env=REDIS_ENDPOINT_URI,REDIS_PASSWORD&envDescription=REDIS_ENDPOINT_URI%20is%20required%20at%20least%20to%20connect%20to%20Redis%20clouding%20server" //Deploy button URL for deploying on Vercel
        },
        {
            "Google": "https://deploy.cloud.run/?git_repo=https://github.com/redis-developer/basic-caching-demo-nodejs.git" //Deploy button URL for deploying on Google cloud.
        }
    ],
    "language": ["JavaScript"], // Backend technologies: "JavaScript", "Java", "Python", "Go", "C#", "Ruby", "PHP", etc. 
    "redis_commands": ["SETEX"], // Enter all the Redis commands
    "redis_features": ["caching"],// Enter any core Redis feature or leave it blank.
    "redis_modules": [], //Value can be one or more of: "RediJSON", "RediSearch", "RedisTimeseries", "RedisAI"  "RedisGears" or "RedisGraph" listed in an array. 
    "app_image_urls": [
        "https://github.com/redis-developer/basic-caching-demo-nodejs/blob/main/docs/screenshot001.png?raw=true"
    ], // Provide any image urls in an array.
    "youtube_url": "", //Provide a Youtube link to your app's video
    "special_tags": [], // "Hackathon", "Paid", or any event names.
    "verticals": ["Healthcare", "Financial"], // Can be: "Healthcare", "Financial", "Tourism", "Retail", "Oil & Gas", "Manufacturing", "Technology","Education", "Construction"  
    "markdown": "https://raw.githubusercontent.com/redislabs-training/redis-sitesearch/master/README.md", // Link to the RAW Markdown.
}
```