<script>
  import logo from './assets/images/logo-universal.png'
  import {GetLocalIp} from '../wailsjs/go/main/App.js'

  let ip = "waiting..."

  function getLocalIp() {
    GetLocalIp().then(result => ip = result)
  }

  getLocalIp()
</script>

<main>
  <h3 id="myip">IP(s): {ip}</h3>
</main>

<style>

  #myip {
    text-align: center;
  }

</style>
