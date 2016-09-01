{% assign rss = site.data.rss-norsk-rally.rss %}

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
						 <div class="t">Nyheter norsk-rally.com</div>
					</div>
			  </div>
			  <div class="BlockContent">
					<div class="BlockContent-body">
					<ul class="unindented">
                        {% for i in (0..4) %}
                            {% assign item = rss.channel.item[i] %}
                            <li>
                                <a href="{{item.link}}" target="_blank">{{item.title}}</a>
                            </li>
                        {% endfor %}
                        </ul>
					</div>
			  </div>
		 </div>
	</div>
