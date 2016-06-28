# contentSlider jQuery Plugin #

contentSlider is a sleek plugin that displays simple animation function using jQuery.

## Version ##
0.1.0

## Usage ## 
    //Switch to next slide
    function nextSlide(){
         $('.active').removeClass('active').addClass('oldActive');
         if($('.oldActive').is(':last-child')){
             $('.slide').first().addClass('active');
        } else {
             $('.oldActive').next().addClass('active');
        }
        $('.oldActive').removeClass('oldActive');
        $('.slide').fadeOut(speed);
        $('.active').fadeIn(speed);
    }     

## Vendors ##
jQuery - [http://jquery.com](http://jquery.com)

## License ##
MIT License
