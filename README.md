# Android-Weather-App

<br>
<p>Este proyecto consiste en la creación de una aplicación para Android usando Kotlin para consultar el clima.
Para obtener la información he usado <a href="https://openweathermap.org" target="_blank">OpenWeatherMap</a> API. 
La API transmite información como temperatura, presión, humedad, estado del tiempo, hora del amanecer y atardecer, etc.
</p>

<b>Creating an Android Weather App using Kotlin</b>
</a>
</p>


<br><h2>Obteniendo una API key para OpenWeatherMap</h2>
<p>Para recuperar datos usaremos <strong>OpenWeatherAPI</strong>, y necesitaremos una clave de la API para ello. Antes de continuar, se debe obtener una clave de la API registrándose en su página.</p>
<ol>
<li>Crear una nueva cuenta en <a title="Create new account" href="https://home.openweathermap.org/users/sign_up" target="_blank" rel="noopener">here</a>.</li>
<li>Después de iniciar sesión ir a <a title="Get the API key" href="https://home.openweathermap.org/api_keys" target="_blank" rel="noopener">here</a> para obtener la API Key.</li>
</ol>

<br><h2>Obteniendo información del clima usando Latitud y Longitud</h2>
<p>Supongamos que desea solicitar información meteorológica utilizando <strong>Latitud</strong> &amp; <strong>Longitud</strong> de un lugar, entonces se debería usar lo siguiente:</p>
<pre>response = URL("https://api.openweathermap.org/data/2.5/weather?lat=$LAT&amp;lon=$LON&amp;units=metric&amp;appid=$API").readText(
                    Charsets.UTF_8
                )</pre>
<p>donde LAT y LON será la Latitud &amp; Longitud respectivamente.
</p>

# weatherAndroidExample
