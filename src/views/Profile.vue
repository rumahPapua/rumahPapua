<template>
  <div class="about">
    <section class="hero is-success is-fullheight">
      <div class="hero-body">
        <div class="container has-text-centered">
            <div class="column is-4 is-offset-4">
                <h3 class="title has-text-black"><a href="https://webwide.io" target="_blank">Webwide</a> Profile Viewer</h3>
                <hr class="login-hr">
                <div class="field is-horizontal userid-label-field">
                  <div class="field-label is-normal">
                    <label class="label">User-ID:</label>
                  </div>
                  <div class="field-body userid-field">
                    <div class="field">
                      <p class="control">
                        <input id="user_id" class="input" type="number" required>
                      </p>
                    </div>
                  </div>
                </div>
                <div class="box">
                  <figure class="avatar">
                      <img id="avatar" src="https://placehold.it/128x128">
                  </figure>
                  <h3 class="title has-text-black"><span id="name">Name</span> <sup><i id="pronoun"></i></sup></h3>
                  <div id="bio"></div>
                  <br>
                  <table class="table details">
                    <tr>
                      <td>Location:</td>
                      <td><span id="location"></span></td>
                    </tr>
                    <tr>
                      <td>Trophy Points:</td>
                      <td><span id="points" class="tag is-info">0</span></td>
                    </tr>
                    <tr>
                      <td>Posts:</td>
                      <td><span id="posts" class="tag is-warning">0</span></td>
                    </tr>
                    <tr>
                      <td>Reactions:</td>
                      <td><span id="reactions" class="tag is-light">0</span></td>
                    </tr>
                    <tr>
                      <td>Moderator:</td>
                      <td><span id="moderator" class="tag is-danger">No</span></td>
                    </tr>
                  </table>
                  <br>
                  <h3 class="is-size-4">Around the web</h3>
                  <table class="table details">
                    <tr>
                      <td>Website:</td>
                      <td><a id="website" href="" target="_blank"></a></td>
                    </tr>
                    <tr>
                      <td>Twitter:</td>
                      <td><a id="twitter" href="" target="_blank"></a></td>
                    </tr>
                    <tr>
                      <td>GitHub:</td>
                      <td><a id="github" href="" target="_blank"></a></td>
                    </tr>
                    <tr>
                      <td>Dribbble:</td>
                      <td><a id="dribbble" href="" target="_blank"></a></td>
                    </tr>
                    <tr>
                      <td>Facebook:</td>
                      <td><a id="facebook" href="" target="_blank"></a></td>
                    </tr>
                    <tr>
                      <td>GitLab:</td>
                      <td><a id="gitlab" href="" target="_blank"></a></td>
                    </tr>
                    <tr>
                      <td>LinkedIn:</td>
                      <td><a id="linkedin" href="" target="_blank"></a></td>
                    </tr>
                    <tr>
                      <td>Behance:</td>
                      <td><a id="behance" href="" target="_blank"></a></td>
                    </tr>
                  </table>
                </div>
                <p class="has-text-grey">
                    <a id="webwide_link" href="https://webwide.io/members/an.19/" target="_blank">View Profile on Webwide.io</a>
                  <br><br>
                  <small><a href="https://twitter.com/AnTheMaker" target="_blank">Webwide Profile Viewer made by <b><i>An</i></b></a></small>
                </p>
            </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style >
  html,body {
  font-family: 'Open Sans', sans-serif;
  font-size: 14px;
  font-weight: 300;
  }
  .hero.is-success {
    background: #F2F6FA;
  }
  .hero .nav, .hero.is-success .nav {
    -webkit-box-shadow: none;
    box-shadow: none;
  }
  #avatar{
    width: 170px;
  }
  #user_id{

  }
  .userid-field{
    flex-grow: 3;
  }
  table.details{
    width: 100%;
  }
  table.details tr td{
    width: 50%;
    word-break: break-all;
  }
  table.details tr td:first-child{
    text-align: right;
    font-weight: bold;
  }
  #bio{
    margin-top: -10px;
    margin-bottom: 20px;
    text-align: fill;
    font-size: small;
    max-width: 100%;
    word-break: break-word;
  }
  #points{
    font-weight: bold;
  }
  #pronoun{
    font-size: 11px;
    opacity: 0.7;
  }
  .box {
    margin-top: 5rem;
  }
  .avatar {
    margin-top: -70px;
    padding-bottom: 20px;
  }
  .avatar img {
    padding: 5px;
    background: #fff;
    border-radius: 50%;
    -webkit-box-shadow: 0 2px 3px rgba(10,10,10,.1), 0 0 0 1px rgba(10,10,10,.1);
    box-shadow: 0 2px 3px rgba(10,10,10,.1), 0 0 0 1px rgba(10,10,10,.1);
  }
  input {
    font-weight: 300;
  }
  p {
    font-weight: 700;
  }
  p.subtitle {
    padding-top: 1rem;
  }

  .login-hr{
    border-bottom: 1px solid black;
  }

  .has-text-black{
    color: black;
  }

  .field{
    padding-bottom: 10px;
  }

  .fa{
    margin-left: 5px;
  }
</style>
