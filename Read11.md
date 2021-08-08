# Read11

## Spring

**Spring FrameWork Means :** *is an open source application framework that provides infrastructure support for developing Java applications, it's the one of the most popular Java Enterprise Edition (Java EE) frameworks.*

## Web controller

**How you can create a web controller?**

>Using @Controller Like:

    package com.example.servingwebcontent;

    import org.springframework.stereotype.Controller;
    import org.springframework.ui.Model;
    import org.springframework.web.bind.annotation.GetMapping;
    import org.springframework.web.bind.annotation.RequestParam;

    @Controller
    public class GreetingController {

        @GetMapping("/greeting")
        public String greeting(@RequestParam(name="name", required=false, defaultValue="World") String name, Model model) {
            model.addAttribute("name", name);
            return "greeting";
        }

    }

**In the home page!!!**

>Using HTML page and `<a href = "/greeting" >` to access the controller should be have a local host to work in it like `http://localhost:5050/` after bach slash adding `greeting` to access it.

