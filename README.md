### Olá! Eu sou o Luiz Eduardo Souza 👋

- 🌱 Estudando Desenvolvimento Web
- 👯 Contate-me no email: oiluizzedu@gmail.com

<div align="center">
  <a href="https://github.com/Luizz-Eduardo">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Luizz-Eduardo&show_icons=true&theme=dracula&include_all_commits=true&count_private=false"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Luizz-Eduardo&layout=compact&langs_count=7&theme=dracula"/>
</div>
  
<div>
   <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg" align="center" alt="Luizz-Js" height="30" width="40">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg" align="center" alt="Luizz-HTML" height="30" width="40">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg" align="center" alt="Luizz-CSS" height="30" width="40" >
</div>
  
<div>
   <a href="https://www.instagram.com/oiluizz_edu/" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
   <a href="https://www.linkedin.com/in/luiz-eduardo-souza-santos-3b6259203/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>
   <a href = "mailto:oiluizzedu@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
</div>
  name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: luizz-eduardo
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  ![Snake animation](https://github.com/Luizz-Eduardo/Luizz-Eduardo/blob/output/github-contribution-grid-snake.svg)
