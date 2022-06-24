<% $foo = "---" %>
author: Gustavo DeLaFuerza
date created: <% tp.date.now("YYYY-MM-DDTHH:mm:ssZ\Z") %>
date modified: <% tp.date.now("YYYY-MM-DDTHH:mm:ssZ\Z") %>
<% $foo = "aliases: daily, daily note, today, yesterday, " + tp.date.now("YYYY-MM-DD") %>
<% $foo = "---" %>