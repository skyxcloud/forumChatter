X-Cloud
Publish the Vendor Assets files by running:

    ```
    php artisan vendor:publish 
    ```

Now that we have published a few new files to our application we need to reload them with the following command:

    ```
    composer dump-autoload
    ```


 Lastly, run the seed files to seed your database with a little data:

    ```
    php artisan db:seed --class=ChatterTableSeeder
    ```

Inside of your master.blade.php file include a header and footer yield. Inside the head of your master or app.blade.php add the following:

    ```
    @yield('css')
    ```

    Then, right above the `</body>` tag of your master file add the following:

    ```
    @yield('js')
    ```