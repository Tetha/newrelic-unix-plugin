newrelic-unix-plugin
====================

New Relic Plugin for monitoring Unix (AIX, BSD, Linux, Solaris) systems

## Installation & Usage ##

1. Download ZIP containing latest JAR: https://github.com/sschwartzman/newrelic-unix-plugin/archive/master.zip
2. Unzip on Unix server that you want to monitor
3. Copy `config/template_newrelic.properties` to `config/newrelic.properties`
4. Copy `config/template_logging.properties` to `config/logging.properties`
4. Edit `config/newrelic.properties`, set your license key
  * License key can be found in New Relic UI, on 'Account settings' page
5. (Optional) Edit `config/unixplugin.config` to set which monitors will be checked (i.e. `df`, `vmstat`, `iostat`)
  * TO DO: list possibilities in this readme
6. Edit `startPlugin.sh` and set `PLUGIN_JAVA_HOME` to location of Java on your server.
7. Run `startPlugin.sh`
8. Check `plugin.log` for errors
9. Check New Relic UI for the "Unix" plugin in left-hand column. Click on it, your instance should appear in the subsequent list.
