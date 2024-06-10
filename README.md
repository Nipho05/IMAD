[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/a7ulFzwn)
  val numbertext = findViewById<EditText>(R.id.editTextNumber)
        findViewById<TextView>(R.id.textView2)
        var message: String
        val button = findViewById<Button>(R.id.button)
         findViewById<Button>(R.id.button2)
        val answer =  findViewById<TextView>(R.id.textView2)

        button?.setOnClickListener{
        val number = numbertext.text.toString().toInt()
            if (number in 20..30)
            {
                message = "The Notorious B.I.G was an american rapper who got shot down in his 20s"
            }
            else if (number in 30..40)
            {
                message = "Bruce Lee was a martial artist who passed away suddenly in his 30s"
            }
            else if (number in 40..50)
            {
                message = "Whitney Houston was a famous singer who passed away in her 40s"
            }
            else
            {
                message = "Invalid number"
            }

            if (number in 20..100)
            {
                answer.text = message
            }
            else
            {
                answer.text = " please enter a number between 20- 100"
            }
        }
    }
}