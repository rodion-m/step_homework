# Буфер обмена
 ```cs
        static Timer StartTimer()
        {
            var timer = new Timer(5000); //5 sec
            timer.Elapsed += OnTimedEvent;
            timer.AutoReset = true;
            timer.Enabled = true;
            return timer;
        }
 ```
