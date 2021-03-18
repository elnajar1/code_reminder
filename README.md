## If you forget a lot like me
> It is better to save the codes that you use often in one place, instead of searching for them on Google every time.

# php
## Curl > get site html content 
`
function get_content($URL){
      $ch = curl_init();
      curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);
      curl_setopt($ch, CURLOPT_URL, $URL);
      $data = curl_exec($ch);
      curl_close($ch);
      return $data;
}
`
