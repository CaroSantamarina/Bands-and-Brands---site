import React from "react";
import { Button } from "@/components/ui/button";
import Image from "next/image";
import Link from "next/link";

export default function HomePage() {
  return (
    <main className="min-h-screen bg-black text-white flex flex-col">
      {/* Navigation */}
      <header className="w-full flex justify-between items-center px-6 py-4 border-b border-gray-700">
        <Image
          src="/bandsandbrands-logo.png"
          alt="Bands and Brands logo"
          width={60}
          height={60}
        />
        <nav className="flex gap-6 text-white text-sm md:text-base">
          <Link href="#about" className="hover:text-gray-300">About</Link>
          <Link href="#how-it-works" className="hover:text-gray-300">How It Works</Link>
          <Link href="#success" className="hover:text-gray-300">Success Stories</Link>
          <Link href="#contact" className="hover:text-gray-300">Contact</Link>
        </nav>
      </header>

      {/* Hero Section */}
      <section className="flex-grow flex flex-col items-center justify-center px-6 text-center py-12">
        <div className="mb-8">
          <Image
            src="/bandsandbrands-logo.png"
            alt="Bands and Brands logo"
            width={200}
            height={200}
            className="mx-auto"
          />
        </div>
        <h1 className="text-4xl md:text-6xl font-bold mb-4">
          Where Music Meets Marketing
        </h1>
        <p className="text-lg md:text-xl text-gray-300 mb-8">
          Bands & Brands is the agency connecting established and emerging artists with powerful
          U.S. brands through unforgettable collaborations.
        </p>
        <div className="flex flex-col sm:flex-row gap-4 justify-center">
          <Button className="bg-white text-black hover:bg-gray-200 px-6 py-3 text-lg">
            For Brands
          </Button>
          <Button className="bg-transparent border border-white text-white hover:bg-white hover:text-black px-6 py-3 text-lg">
            For Bands
          </Button>
        </div>
      </section>

      {/* How It Works Section */}
      <section id="how-it-works" className="bg-gray-950 text-white py-16 px-6">
        <div className="max-w-5xl mx-auto text-center">
          <h2 className="text-3xl md:text-4xl font-bold mb-6">How It Works</h2>
          <div className="grid md:grid-cols-3 gap-10 text-left">
            <div className="bg-gray-900 p-6 rounded-2xl shadow-md">
              <h3 className="text-xl font-semibold mb-2">1. Discover</h3>
              <p className="text-gray-300">
                Brands tell us what they’re looking for, and we handpick bands that align with their values and target market.
              </p>
            </div>
            <div className="bg-gray-900 p-6 rounded-2xl shadow-md">
              <h3 className="text-xl font-semibold mb-2">2. Connect</h3>
              <p className="text-gray-300">
                We facilitate direct connections, negotiate partnerships, and manage logistics for smooth collaboration.
              </p>
            </div>
            <div className="bg-gray-900 p-6 rounded-2xl shadow-md">
              <h3 className="text-xl font-semibold mb-2">3. Amplify</h3>
              <p className="text-gray-300">
                From campaigns to live events, we help amplify your brand and the artist’s reach through strategic exposure.
              </p>
            </div>
          </div>
        </div>
      </section>

      {/* Success Stories Section */}
      <section id="success" className="bg-black text-white py-16 px-6">
        <div className="max-w-5xl mx-auto text-center">
          <h2 className="text-3xl md:text-4xl font-bold mb-10">Success Stories</h2>
          <div className="grid md:grid-cols-2 gap-10 text-left">
            <div className="bg-gray-900 p-6 rounded-2xl shadow-md">
              <h3 className="text-xl font-semibold mb-2">Indie Band × Beverage Brand</h3>
              <p className="text-gray-300">
                A rising indie band partnered with a national beverage company for a summer tour, boosting brand engagement by 40%.
              </p>
            </div>
            <div className="bg-gray-900 p-6 rounded-2xl shadow-md">
              <h3 className="text-xl font-semibold mb-2">Pop Artist × Fashion Label</h3>
              <p className="text-gray-300">
                A pop artist’s merch line sold out in under 24 hours after collaborating with a fast-fashion brand on a capsule collection.
              </p>
            </div>
            <div className="bg-gray-900 p-6 rounded-2xl shadow-md">
              <h3 className="text-xl font-semibold mb-2">DJ Collective × Tech Startup</h3>
              <p className="text-gray-300">
                A tech startup gained viral traction after syncing its app launch with exclusive DJ events across college campuses.
              </p>
            </div>
            <div className="bg-gray-900 p-6 rounded-2xl shadow-md">
              <h3 className="text-xl font-semibold mb-2">Singer-Songwriter × Eco Brand</h3>
              <p className="text-gray-300">
                A sustainable lifestyle brand tapped a soulful artist for its Earth Day campaign, resulting in record-breaking online engagement.
              </p>
            </div>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer id="contact" className="bg-gray-900 text-gray-400 text-sm text-center py-4">
        &copy; {new Date().getFullYear()} Bands and Brands. All rights reserved.
      </footer>
    </main>
  );
}
