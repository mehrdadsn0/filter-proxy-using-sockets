# filter-proxy
this is a http proxy server to prevent accessing certain websites (not working on https)

برنامه اي به عنوان سرور نوشته مي‌شود كه يك درخواست HTTP كه از مرورگر ارسال شده را گرفته و مشخصات مقصد را از آن استخراج مي‌نمايد. از فايلي متني كه حاوي اطلاعات سايت‌هاي فيلتر شده مي‌باشد اطلاعات آن سايت را جستجو خواهد كرد. اگر در فايل وجود نداشت ارتباط با سايت مورد نظر را برقرار كرده و درخواست را ارسال نموده و پاسخ را تحويل كلاينت(مرورگر) خواهد داد. اگر سايت فيلتر شده بود بايستي صفحه HTMLي ثابتي كه براي خطاي فيلتر در سرور قرار دارد را به كلاينت ارسال نمايد.
هر سطر فايل فيلتر معرفي يك فيلتر مي‌باشد. محتويات فايل فيلتر مي‌تواند داراي * باشد كه به معني همه است براي مثال:
1-	اگر www.iaut.ac.ir در فايل باشد يعني فقط هاست مربوطه به آن آدرس فيلتر مي باشد و مابقي آدرس‌هاي آن دامنه مثل mail.iaut.ac.ir فيلتر نمي‌باشد.
2-	اگر *.iaut.ac.ir در فايل باشد يعني همه هاست‌هاي آن دامنه فيلتر است.
3-	اگر *.ir باشد يعني همه دامنه‌هاي ir فيلتر مي‌باشد.
4-	اگر *.* باشد همه سايت‌ها فيلتر است.
