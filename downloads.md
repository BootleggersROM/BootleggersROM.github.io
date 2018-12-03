---
layout: default
title: Downloads
---
<div class="card shishu-light-bg z-depth-3">
  <div class="card-content">
    <span class="card-title">Welcome to our downloads</span>
    <p>This is where all our officially supported devices are listed. If the device you're looking for isn't on the list, please check your build type (all the official releases are Shishufied) or ask your device maintainer to talk to us on our <a href="https://t.me/keepthebootleg">Telegram Chat.</a> Also, you can check our <a href="{{- 'extras/addons' | relative_url -}}">suggested addons and apps</a> that you might find interesting.</p>
  </div>
</div>
<div class="card shishu-light-bg z-depth-3">
  <div class="card-content">
    <span class="card-title">Releases</span>
    <ul class="collapsible shishu-lighter-bg collapsible-noborder">
      {% for device in site.devices %}
        <li>
          <div class="collapsible-header collapsible-noborder shishu-lighter-bg">
            <i class="material-icons">phone_android</i>
          {{ device.codename }} | {{ device.fullname }}</div>
          <div class="collapsible-body collapsible-noborder shishu-midlight-bg">
            <span>Maintainer:</span><div class="chip shishu-lighter-bg" style="margin-left:4px">{{ device.maintainer }}</div><br>
            <span>Latest build:</span><div class="chip shishu-lighter-bg" style="margin-left:4px">{{ device.filename }}</div><br>
            <span>Build size:</span><div class="chip shishu-lighter-bg" style="margin-left:4px">{{ device.buildsize }}</div><br><br>
            <a class="waves-effect waves-light btn-small shishu-accent-btn" href="https://sourceforge.net/projects/bootleggersrom/files/builds/{{ device.codename }}/{{ device.filename }}"><i class="material-icons left">get_app</i>Download</a>
            {% if device.mirrorlink %}
              <a class="waves-effect waves-light btn-small shishu-accent-btn" href="{{ device.mirrorlink }}"><i class="material-icons left">open_in_new</i>Mirror</a>
            {% endif %}
            <a class="waves-effect waves-light btn-small shishu-accent-btn" href="https://sourceforge.net/projects/bootleggersrom/files/builds/{{ device.codename }}"><i class="material-icons left">history</i>Older Builds</a>
            {% if device.xdathread %}
              <a class="waves-effect waves-light btn-small shishu-accent-btn" href="{{ device.xdathread }}"><i class="material-icons left">library_books</i>XDA Thread</a>
            {% endif %}
          </div>
        </li>
      {% endfor %}
    </ul>
  </div>
</div>
{% for post in site.posts %}
{% endfor %}