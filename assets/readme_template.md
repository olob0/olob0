<div align="center">
  <h3>👋 Olá, eu sou o {{ gh_name }}</h3>
  
  <p>🐺 Me chamo Gabriel Loboㅤㅤㅤㅤㅤ</p>
  <p>🧔 Eu tenho {{ '2006-07-02' | age }} anosㅤㅤㅤㅤㅤㅤㅤㅤ</p>
  <p>🧠 Sou um entusiasta de tecnologia</p>

  <br/>

  <img width="600" alt="Skills / cool things" src="https://skills-icons.vercel.app/api/icons?i=python,md,html,css,js,github,git,vscode,linux,node,ts,sass,react,vite,vercel,lottie,ionic,capacitor,zustand,framer,firebase,arduino,godot,tailwind,shadcnui,lucide,zorinos,pnpm,reactnative&perline=14" />
</div>

<hr />

{% if followers|length > 0 %}
<div align="center">
    <h4>👤 Seguidores 👤</h4>
    <p><i>Gostaria de participar? Só me seguir!</i></p>
    <img width="600" src=".github/assets/cards/top3.svg" alt="Top 3 followers contributors (monthly)" />
    {% if followers|length > 2 and total_contributions > 0 %}
    <details>
    <summary>🏅 Classificações 🏅</summary>
    <br/>
    <table>
        <thead>
            <tr align="center">
                <th>Posição</th>
                <th>Seguidor</th>
                <th>Contribuições</th>
            </tr>
        </thead>
        <tbody>
            {% for position, name, url, contributions in followers %}
            {% if contributions > 0 %}
            <tr align="center">
                <td>{{ position }}°</td>
                <td><a href="{{ url }}">{{ name }}</a></td>
                <td>{{ contributions }} ctr.</td>
            </tr>
            {% endif %}
            {% endfor %}
        </tbody>
    </table>
    </details>
    {% endif %}
</div>
{% endif %}

<div align="center">
  <h4>🐍 Snakommits 🐍</h4>
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/olob0/olob0/snake-output/snake-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/olob0/olob0/snake-output/snake-light.svg">
      <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/olob0/olob0/snake-output/snake-light.svg">
    </picture>
</div>

<h6 align="right">
  Esse perfil é atualizado diariamente!<br/> <i>{{ last_update }}</i>
<h6>
