# Cusotm Post Status

Easily create custom post statuses within WordPress for one or more custom post types.

## Usage

```php
new CustomPostStatus($post_status, $post_types, $args);
```

### Parameters

1. __$post_status__ (string) Required. Machine name of the post status; for example, "archive"
2. __$post_types__ (array) Optional. Array of post types to apply the post status to. Default: ["post"]
3. __$args__ (array) Optional. Array of arguments. All arguments from [register_post_status](http://codex.wordpress.org/Function_Reference/register_post_status) plus:
    - __applied_label__ (string) Optional. Status label used when the user has applied this post status (for example, "Archived"). Default: $args["label"] || $post_status
