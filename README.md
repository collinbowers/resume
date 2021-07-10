# resume
Used to host my up-to-date resume.

I used [json resume](https://jsonresume.org/getting-started/) to create a resume in json format. Then I used [js-yaml](https://www.npmjs.com/package/js-yaml) to convert that json file into a pretty yaml file. I then chose a theme to use from [here](https://jsonresume.org/themes/). And deployed it all to github pages. 

```
npm install
npm init
npm install -g gh-pages resume-cli npm-watch js-yaml {and dont forget to install the theme that you choose} 

## this will init a resume-json file which you can edit with your resume info
resume init

## once you've built out your resume
js-yaml resume.json > resume.yaml
```

Lastly, check out my scripts in my package.json, and plug and play what you need to. Essentially i create a public folder, export my resume into an html file within that folder, and deploy that folder to gh-pages. Pretty easy! 
