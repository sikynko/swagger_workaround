# swagger_workaround

If you dont want to reach swagger from url http://<your-host-name/swagger-ui.html but you want reach something different.
http://<your-host-name/index or another.
```java
1. Create controller which will point to your url. 
@Controller
public class SwaggerUIRedirectController {

    @RequestMapping("/index")
    public String uiRedirectLink() {
        return "index";
    }

}
```

2. copy html and js file
