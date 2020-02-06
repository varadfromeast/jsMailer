var nodemailer = require('nodemailer');

var transporter = nodemailer.createTransport({
  service: 'gmail',
  auth: {
    user: 'sih.codewarriors@gmail.com',
    pass: 'sih2020cw'
  }
});

var mailOptions = {
  from: 'sih.codewarriors@gmail.com',
  to: 'shubhankargaikwad2006@gmail.com, sidheehande@gmail.com',
  subject: 'Sending Email using Node.js',
  text: 'That was easy!',
  attachments:[
  {
	  filename:'TE-Comp-Syllabus.pdf',
	  path:'C:/Users/S Gaikwad/js-projects/TE-Comp-Syllabus.pdf',
	  contentType:'application/pdf'
	  
	  
  }
  ]
};

transporter.sendMail(mailOptions, function(error, info){
  if (error) {
    console.log(error);
  } else {
    console.log('Email sent: ' + info.response);
  }
});