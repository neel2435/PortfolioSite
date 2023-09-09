<script>
    let title = "Neel Doshi"
</script>

<div class="topnav">
    <img src="/whitecomp.png" alt="site logo" class="logo">
    <ul>
        <li><a href="/">Home</a></li>
        <li>
          <div class="icon-wrapper">
            <a href="https://www.linkedin.com/in/neel-doshi-5356a3205/" class="icon-link">
              <img src="/icons8-linkedin-50.png" alt="LinkedIn" class="icon-linked" />
            </a>
          </div>
        </li>
        <li>
          <div class="icon-wrapper">
            <a href="https://github.com/neel2435" class="icon-link">
              <img src="/icons8-github-50.png" alt="GitHub" class="icon-git" />
            </a>
          </div>
        </li>
        <li><a href="/about">About</a></li>
    </ul>
</div>

<style>
.topnav {
  background-color: rgb(0, 0, 0);
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  box-shadow: 0 0 25px 0 rgb(0, 0, 0);
}

.topnav ul {
  display: flex;
  align-items: center;
  margin: 0;
  padding: 0;
}

.topnav li {
  margin: 0 30px;
  list-style: none;
}

.topnav a {
  color: rgb(255, 255, 255);
  transition: color 0.5s ease;
  text-decoration: none;
  font-size: 1rem;
  font-family: monospace;
  vertical-align: middle;
}

.topnav .icon-wrapper {
  display: inline-block;
  transition: background-color 0.5s ease;
}

.topnav a:hover {
  color: rgb(99, 236, 154);
}

.icon-wrapper:hover .icon-git {
    content: url('/icons8-github-51.png')
}

.icon-wrapper:hover .icon-linked {
    content:url('/icons8-linkedin-51.png')
}

.icon-git {
  display: block;
  width: 25px;
  height: 25px;
  filter: none;
}

.icon-linked {
  display: block;
  width: 25px;
  height: 25px;
  filter: none;
}

.topnav img {
  vertical-align: middle;
}

.topnav .logo {
    width: 25px;
    height: 25px;
    padding: 16px 16px;
    padding-left: 35px;
}
</style>