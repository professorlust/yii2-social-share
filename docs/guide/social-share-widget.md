Social share widget
===================

## Configuration options

| Option | Description | Type | Default |
|--------|-------------|------|---------|
|configuratorId|ID of configurator component from app config|string|-|
|url|Absolute URL to share page|string|Result of `Url::to('', true)`|
|title|Title of share page|string|-|
|description|Description of share page|string|-|
|imageUrl|Absolute URL to image for share page|string|-|
|wrapperTag|Wrapper HTML tag name for all share links|string|ul|
|wrapperOptions|HTML options for wrapper tag|array|`['class' => 'social-share']`|
|linkWrapperTag|Wrapper HTML tag name for one share link|bool/string|li|
|linkWrapperOptions|HTML options for link wrapper tag|array|-|