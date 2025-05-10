import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Download, Mail, Users } from "lucide-react";

export default function Home() {
  return (
    <div className="min-h-screen bg-white text-gray-800 p-4 md:p-10 space-y-16">
      {/* Hero Section */}
      <section className="text-center space-y-4">
        <img
          src="/logo.png"
          alt="UOHC Logo"
          className="mx-auto w-32 md:w-40 rounded-full shadow-md"
        />
        <h1 className="text-4xl md:text-5xl font-bold text-blue-900">
          United Oromo Hararge Community (UOHC)
        </h1>
        <p className="text-gray-700 text-lg max-w-2xl mx-auto">
          Empowering the Oromo Hararge community through unity, education,
          cultural pride, and newcomer support in Edmonton and beyond.
        </p>
        <Button className="mt-4 bg-blue-700 hover:bg-blue-800 text-white px-6 py-2 rounded-full shadow">
          Join Us
        </Button>
      </section>

      {/* About Section */}
      <section className="grid md:grid-cols-2 gap-8">
        <Card className="bg-gray-50 border border-gray-200 shadow">
          <CardContent className="p-6 space-y-4">
            <h2 className="text-2xl font-semibold text-blue-700">Our Mission</h2>
            <p>
              We aim to uplift Oromo Hararge people through charitable,
              educational, and cultural programs. We assist newcomers in
              settling and thriving in Canada while preserving our heritage.
            </p>
          </CardContent>
        </Card>

        <Card className="bg-gray-50 border border-gray-200 shadow">
          <CardContent className="p-6 space-y-4">
            <h2 className="text-2xl font-semibold text-blue-700">What We Do</h2>
            <ul className="list-disc pl-6 space-y-2 text-gray-700">
              <li>Support newcomers with settlement services</li>
              <li>Educate and empower youth about culture and leadership</li>
              <li>Organize events, celebrations, and fundraising</li>
              <li>Apply for government grants and community sponsorships</li>
              <li>Keep members informed every 4 months</li>
            </ul>
          </CardContent>
        </Card>
      </section>

      {/* Membership and Programs */}
      <section className="grid md:grid-cols-3 gap-8">
        <Card className="bg-white border border-gray-200 shadow">
          <CardContent className="p-6">
            <h3 className="font-bold text-lg text-blue-700 mb-2">Membership</h3>
            <p className="text-sm text-gray-600 mb-4">
              Become a member and contribute annually to keep our community
              thriving. Members who do not pay their annual fees will be
              suspended.
            </p>
            <Button><Users className="mr-2 w-4 h-4" /> Become a Member</Button>
          </CardContent>
        </Card>

        <Card className="bg-white border border-gray-200 shadow">
          <CardContent className="p-6">
            <h3 className="font-bold text-lg text-blue-700 mb-2">Donate</h3>
            <p className="text-sm text-gray-600 mb-4">
              Support our cultural events, youth programs, and newcomer
              services by donating generously.
            </p>
            <Button variant="outline">Donate Now</Button>
          </CardContent>
        </Card>

        <Card className="bg-white border border-gray-200 shadow">
          <CardContent className="p-6">
            <h3 className="font-bold text-lg text-blue-700 mb-2">Community Bylaws</h3>
            <p className="text-sm text-gray-600 mb-4">
              Download our official bylaws and community regulation document.
            </p>
            <Button variant="secondary">
              <Download className="mr-2 w-4 h-4" />
              <a href="/UOHC_Bylaws_StrategicPlan_Styled.pdf" download>
                Download PDF
              </a>
            </Button>
          </CardContent>
        </Card>
      </section>

      {/* Contact */}
      <section className="text-center pt-10">
        <h2 className="text-2xl font-bold text-blue-800">Get in Touch</h2>
        <p className="text-gray-700">Email us: arifadam616@gmail.com</p>
        <Button variant="link" className="mt-2">
          <Mail className="mr-2 w-4 h-4" /> Send Email
        </Button>
      </section>

      {/* Footer */}
      <footer className="text-center text-sm text-gray-500 pt-10 border-t mt-10">
        &copy; {new Date().getFullYear()} United Oromo Hararge Community. All rights reserved.
      </footer>
    </div>
  );
}
