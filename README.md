# bStats-PMMP
> bStats-PMMP is an implementation of bStats (https://bStats.org) for PocketMine.

## How to use:

```php
namespace your\name\space;

use pocketmine\plugin\PluginBase;
use xxFLORII\bStats\Metrics;

class YourPlugin extends PluginBase {
    
    protected function onEnable() : void{
        $pluginId = 1234; //ToDo: replace with your plugin ID from https://bstats.org
        $metrics = new Metrics($this, $pluginId);
        $metrics->scheduleMetricsDataSend();
    }
}
```