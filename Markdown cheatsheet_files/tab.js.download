
       $(".tab_content").hide();
       $(".tab_container").each(function() {
         $( this ).children(".tab_content").first().show();
      });
      $(".tabs").each(function() {
        $( this ).children().first().addClass("active");
     });

     /* if in tab mode */
       $("ul.tabs li").click(function() {

         var activeTab = $(this).attr("rel");
          $("#"+activeTab).siblings('.tab_content').hide();
         $("#"+activeTab).slideDown(200);

         $(this).siblings().removeClass("active");
         $(this).addClass("active");


       });
     /* if in drawer mode */
     $(".tab_drawer_heading").click(function() {


         var d_activeTab = $(this).attr("rel");
         $("#"+d_activeTab).siblings('.tab_content').hide();
         $("#"+d_activeTab).slideDown(200);

         $(this).siblings(".tab_drawer_heading").removeClass("d_active");
         $(this).addClass("d_active");

       $("ul.tabs li").removeClass("active");
       $("ul.tabs li[rel^='"+d_activeTab+"']").addClass("active");
       });
