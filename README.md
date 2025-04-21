git clone https://github.com/PennySense/penny-sense-site.git
import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import Image from "next/image";

export default function HomePage() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-green-50 to-white p-4 text-brown-900">
      <header className="text-center py-8">
        <div className="flex justify-center items-center space-x-4 mb-4">
          <Image
            src="/logo.png"
            alt="Penny Sense Logo"
            width={60}
            height={60}
            className="rounded-full"
          />
          <div>
            <h1 className="text-5xl font-bold text-brown-800">Penny Sense</h1>
            <p className="text-xl italic text-brown-600">"Making Our Pennies Make Cents"</p>
          </div>
        </div>
      </header>

      <nav className="flex justify-center space-x-4 mb-8">
        <a href="#about" className="text-green-700 hover:underline">About Us</a>
        <a href="#services" className="text-green-700 hover:underline">Services</a>
        <a href="#team" className="text-green-700 hover:underline">Team</a>
        <a href="#testimonials" className="text-green-700 hover:underline">Testimonials</a>
        <a href="#contact" className="text-green-700 hover:underline">Contact</a>
      </nav>

      <section id="about" className="max-w-4xl mx-auto space-y-6">
        <Card className="bg-white shadow-xl rounded-2xl p-6">
          <CardContent>
            <h2 className="text-2xl font-semibold text-green-800">About Us</h2>
            <p className="mt-4 text-brown-700">
              Rumor has it, finding money in the form of coins carries a powerful spiritual meaning. Some believe it to be a form of angelic messages from one of our ancestors to communicate with us. To interpret the message, experts suggest that one add the numbers of the date printed on the coin and use numerology to decode the message.
            </p>
            <p className="mt-2 text-brown-700">
              For over a year, Jerome R. Wilson, CEO and founder of Penny Sense, kept finding pennies thrown out on the streets. He began saving them in an old coffee can jar, a nod to the classic "coffee can portfolio" investment strategy. Just like those pennies, penny stocks are often discarded on Wall Street — overlooked and undervalued.
            </p>
            <p className="mt-2 text-brown-700">
              Penny Sense is committed to picking up these discarded penny stocks and preserving them in long-term Coffee Can Portfolios, thus “Making Our Pennies Make Cents.”
            </p>
          </CardContent>
        </Card>

        <Card id="services" className="bg-white shadow-xl rounded-2xl p-6">
          <CardContent>
            <h2 className="text-2xl font-semibold text-green-800">Services</h2>
            <p className="mt-4 text-brown-700">
              We produce a YouTube broadcast and podcast highlighting Coffee Can Portfolios featuring the most oversold penny stocks on Wall Street. Our goal is to inspire and educate novice investors and young traders on the value of patience, long-term holding, and the power of compounding.
            </p>
          </CardContent>
        </Card>

        <Card id="team" className="bg-white shadow-xl rounded-2xl p-6">
          <CardContent>
            <h2 className="text-2xl font-semibold text-green-800">Team</h2>
            <p className="mt-4 text-brown-700">
              <strong>Jerome R. Wilson</strong> – CEO & Founder. A visionary investor with a passion for uncovering the value in what others throw away. Jerome created Penny Sense from personal experience and a deeper understanding of financial growth through compounding.
            </p>
          </CardContent>
        </Card>

        <Card id="testimonials" className="bg-white shadow-xl rounded-2xl p-6">
          <CardContent>
            <h2 className="text-2xl font-semibold text-green-800">Testimonials</h2>
            <p className="mt-4 text-brown-700 italic">“Penny Sense changed the way I look at investing. Jerome's approach is simple but powerful.” – A. Young Investor</p>
            <p className="mt-2 text-brown-700 italic">“The Coffee Can Portfolio philosophy is genius. I actually feel like I’m building wealth now.” – B. Newbie Trader</p>
            <p className="mt-2 text-brown-700 italic">“Before Penny Sense, I had no idea what to do with penny stocks. Now I feel empowered to make informed decisions.” – C. Budget Investor</p>
            <p className="mt-2 text-brown-700 italic">“I love the mission behind this company. It’s more than just numbers—it’s about mindset and value.” – D. Aspiring Entrepreneur</p>
            <p className="mt-2 text-brown-700 italic">“Jerome is an incredible teacher. His stories make investing feel relatable and achievable.” – E. Everyday Worker</p>
          </CardContent>
        </Card>

        <Card id="contact" className="bg-white shadow-xl rounded-2xl p-6">
          <CardContent>
            <h2 className="text-2xl font-semibold text-green-800">Contact Us</h2>
            <form
              className="mt-4 space-y-4"
              action="https://formsubmit.co/pennysense.tv@gmail.com"
              method="POST"
            >
              <input className="w-full p-2 border rounded" type="text" name="name" placeholder="Your Name" required />
              <input className="w-full p-2 border rounded" type="email" name="email" placeholder="Your Email" required />
              <textarea className="w-full p-2 border rounded" name="message" placeholder="Your Message" rows="4" required></textarea>
              <input type="hidden" name="_captcha" value="false" />
              <Button type="submit" className="bg-green-700 text-white px-4 py-2 rounded">Send Message</Button>
            </form>
            <div className="mt-6">
              <p className="text-brown-700">Follow us on social media:</p>
              <a href="https://www.facebook.com/PennySense" target="_blank" className="text-green-700 hover:underline">Facebook: PennySense</a>
            </div>
          </CardContent>
        </Card>

        <div className="flex justify-center">
          <Button className="bg-green-700 text-white text-lg px-6 py-2 rounded-full shadow-md">
            Learn More
          </Button>
        </div>
      </section>
    </div>
  );
}
cd penny-sense-site
git add .
git commit -m "Initial Penny Sense site"
git push origin main
