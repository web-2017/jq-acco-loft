$(function(){
    
    $('.acco__trigger').on('click', function(e){
        e.preventDefault();

        var $this = $(this),
            container = $this.closest('.acco'),
            otherContent = container.find('.acco__content'),
            items = container.find('.acco__item'),
            item = $this.closest('.acco__item'),
            content = item.find('.acco__content'),
            reqHeight = item.find('.acco__content-text').outerHeight();

            if(!item.hasClass('active')){
                items.removeClass('active');
                item.addClass('active');

                otherContent.css({
                    'height': 0
                });

                content.css({
                    'height': reqHeight
                });
            } else{
                item.removeClass('active');
                content.css({
                    'height': 0
                });
            }

    });
    
});
