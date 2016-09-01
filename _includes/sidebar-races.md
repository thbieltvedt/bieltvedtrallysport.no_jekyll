{% assign previous-race = site.data.races.previous-race %}
{% assign next-race = site.data.races.next-race %}

<div class="Block">
     <div class="Block-tl"></div>
     <div class="Block-tr"></div>
     <div class="Block-bl"></div>
     <div class="Block-br"></div>
     <div class="Block-tc"></div>
     <div class="Block-bc"></div>
     <div class="Block-cl"></div>
     <div class="Block-cr"></div>
     <div class="Block-cc"></div>
     <div class="Block-body">
          <div class="BlockHeader">
                <div class="l"></div>
                <div class="r"></div>
                <div class="header-tag-icon">
                     <div class="t">Løp</div>
                </div>
          </div>
          <div class="BlockContent">
                <div class="BlockContent-body">
                    {% if next-race %}
                        <p style="margin-bottom: 4px; font-size: 11px; font-weight: bold">Neste løp:</p>
                        <p style="margin: 0px;"><a href="{{next-race.hjemmeside-url}}" target="_blank">{{next-race.navn}}</a></p>
                        <p style="margin: 0px;">{{next-race.dato}}</p>
                        <br/>
                    {% endif %}
                    {% if previous-race %}
                        <p style="margin-bottom: 4px; font-size: 11px; font-weight: bold">Forrige løp:</p>
                        <p style="margin: 0px;"><a href="{{previous-race.hjemmeside-url}}" target="_blank">{{previous-race.navn}}</a></p>
                        <p style="margin: 0px;">{{previous-race.dato}}</p>
                    {% endif %}
                </div>
          </div>
     </div>
</div>