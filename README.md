
<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

<!--h1 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h1 style="display: inline-block">Hi 👋, I'm Mehdi</h1></summary>
  </ul>
</div>


<!--- snake -->
name: GitHub Snake Game

on:
  # Schedule the workflow to run daily at midnight UTC
  schedule:
    - cron: "0 0 * * *"
  # Allow manual triggering of the workflow
  workflow_dispatch:
  # Trigger the workflow on pushes to the main branch
  push:
    branches:
      - main
jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10
    steps:
      # Step 1: Checkout the repository
      - name: Checkout Repository
        uses: actions/checkout@v3
      # Step 2: Generate the snake animations
      - name: Generate GitHub Contributions Snake Animations
        uses: Platane/snk@v3
        with:
          # GitHub username to generate the animation for
          github_user_name: ${{ github.repository_owner }}
          # Define the output files and their configurations
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark
            dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
      # Step 3: Deploy the generated files to the 'output' branch
      - name: Deploy to Output Branch
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./dist
          publish_branch: output
          # Optionally, you can set a custom commit message
          commit_message: "Update snake animation [skip ci]"


<!--h2 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Confusion is part of Programming</h2></summary>
  </ul>
</div>


<!--Intro start-->
- 🔭 I’m currently working on **Full stack web develpement/ IoT / UI|UX Design**

- 🌱 I’m currently learning **machine learning / big data mining**

- 📫 Feel free to reach me out **km_mamouni@esi.dz**


<!--Intro end-->



<!--- stats & Trophy (start) -->
<p align="center">
  <!--- stats (start) -->
<table align="center">
<tr border="none">
<td width="50%" align="center">
  
  <img  align="center"  src="https://github-readme-stats.vercel.app/api?username=thenotoriousmehdi&theme=dark&show_icons=true&count_private=true" />
  <br></br>
  <img  title="🔥 Get streak stats for your profile at git.io/streak-stats" alt="Mark streak" src="http://github-readme-streak-stats.herokuapp.com?user=thenotoriousmehdi&theme=dark" /> 
</td>

<td width="50%" align="center">

  <img  align="center"  src="https://github-readme-stats.anuraghazra1.vercel.app/api/top-langs/?username=thenotoriousmehdi&theme=dark&hide_border=false&no-bg=true&no-frame=true&langs_count=10"/>
  
  </td>
</tr>
</table>
<!--- stats (end) -->







<!--h1 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Technologies That I Know👨🏻‍💻</h2></summary>
  </ul>
</div>
<!--tech stack icons-->
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=git,c,css,discord,figma,github,html,idea,java,js,linux,materialui,react,tailwind, react,tailwind,vscode&perline=14" />
  </a>
</p>


<!-- Connect with me -->
<!--h2 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Connect With Me🤝</h2></summary>
  </ul>
</div>

<!--icons and links-->
<p align="center">
<a href="https://www.linkedin.com/in/mehdi-mamouni-68a010211/" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234979284-68c11d7f-1acc-4f0c-ac78-044e1037d7b0.png" alt="linkedin" height="50" width="50" /></a>

</p>


<!--profile visit count-->
<div align="center">
  
<a href="https://visitcount.itsvg.in">
  <img src="https://visitcount.itsvg.in/api?id=thenotoriousmehdi&label=Profile%20Views&pretty=true" />
</a>
  
</div>

<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

----------------------------------------------------------------------

