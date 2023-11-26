const transporter = nodemailer.createTransport({ 
    host: 'smtp.example.com',
    port: 465,
    secure: true,
    auth: { 
        user: 'user@example.com',
        pass: 'password'
        }
        })

transporter.sendMail(
    { 
    from: 'sender@example.com',
    to: 'recipient@example.com',
    subject: 'Hello',
    text: 'Hello, world!' 
    }
    );