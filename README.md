# jq-acco-loft

            <ul class="acco">

                <li class="acco__item">
                    <a href="#" class="acco__trigger">Пункт 1</a>
                    <div class="acco__content">
                        <div class="acco__content-text">
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium laborum rem dolorem. Hic, reiciendis. Dolores saepe fuga enim, consectetur assumenda!
                        </div>
                    </div>
                </li>

                <li class="acco__item">
                    <a href="#" class="acco__trigger">Пункт 2</a>
                    <div class="acco__content">
                        <div class="acco__content-text">
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Atque ipsum vero, possimus neque recusandae maxime magni numquam quidem ullam voluptas assumenda quas, mollitia praesentium rerum ea eum dolores et quis fugiat minus excepturi animi iusto nihil suscipit. Porro, aut, tempore.
                        </div>
                    </div>
                </li>

                <li class="acco__item">
                    <a href="#" class="acco__trigger">Пункт 3</a>
                    <div class="acco__content">
                        <div class="acco__content-text">
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quae aliquam ut velit! Minima error ut pariatur quasi fuga recusandae facere molestiae beatae totam, nihil hic tempora quos officiis officia adipisci ullam explicabo, accusantium aliquid enim placeat iusto id animi, facilis labore omnis. Quam magnam mollitia nisi odio, dolore eaque aliquam distinctio, voluptatibus ea molestias ducimus harum veritatis laudantium ad voluptatum. Unde voluptatum tempore aperiam tenetur neque dolorem est perferendis. Explicabo maiores nemo velit nisi debitis quam adipisci tempore nostrum odio?
                        </div>
                    </div>
                </li>

                <li class="acco__item">
                    <a href="#" class="acco__trigger">Пункт 4</a>
                    <div class="acco__content">
                        <div class="acco__content-text">
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Possimus, inventore, consequatur? Architecto saepe mollitia ex quas excepturi similique, ut minima vero quaerat, doloremque reprehenderit odio, officia. Aut voluptatem facilis atque pariatur molestias doloribus consectetur minima inventore nam eaque, harum labore eos odit quo quos quaerat reprehenderit ad exercitationem repellendus totam sapiente quidem numquam. Dicta, recusandae, corrupti veniam, magnam pariatur ducimus odio, laboriosam porro vero ex optio quo beatae alias. Aliquid, incidunt culpa fugiat! Assumenda ipsam id quo, dolor ea laborum aperiam voluptates excepturi nemo quae. Molestias quibusdam laudantium, dolore ipsum, incidunt sint. Recusandae hic suscipit, dolorum repellendus aspernatur dolor quod!
                        </div>
                    </div>
                </li>

            </ul>
            
            <script>
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
    </script>
