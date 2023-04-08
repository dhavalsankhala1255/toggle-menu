<div class="menu-toggle">
    <span class="bar1"></span>
    <span class="bar2"></span>
    <span class="bar3"></span>
</div>

/*---- css -----*/

.menu-toggle {
    display: none;
}

/*----responsive---*/

.menu-toggle {
        display: flex;
        flex-wrap: wrap;
        width: 40px;
        height: 28px;
        z-index: 9;
        position: relative;
        margin-left: auto;
    }
    .menu-toggle span {
        width: 30px;
        height: 3px;
        background: #000;
        transition: all 0.3s;
        backface-visibility: hidden;
        display: block;
    }
    .menu-toggle span:first {
        margin-top: 0;
    }
    .menu-toggle:focus {
        outline: none;
    }
    .menu-toggle.on .bar1 {
        transform: rotate(45deg) translate(6px, 5px);
    }
    .menu-toggle.on .bar2 {
        opacity: 0;
    }
    .menu-toggle.on .bar3 {
        transform: rotate(-45deg) translate(8px, -8px);
    }
    .navbar {
        display: none;
        position: absolute;
        top: 60px;
        right: 0;
    }
    .navbar ul {
        display: block;
        padding: 15px;
        background: #fff;
        width: 300px;
        height: 300px;
        position: relative;
        box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
        z-index: 2;
    }
    
    /*-------JS------/
    $(".menu-toggle").click(function() {
        $(this).toggleClass("on");
        $(".navbar").slideToggle();
    });
