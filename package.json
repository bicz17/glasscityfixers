import { useState } from 'react';
import { motion } from 'framer-motion';


export default function Home() {
const [formData, setFormData] = useState({ name: '', phone: '', address: '', service: '' });


const handleChange = (e) => {
setFormData({ ...formData, [e.target.name]: e.target.value });
};


const handleSubmit = (e) => {
e.preventDefault();
alert('Thanks! We received your request and will reach out shortly.');
};


return (
<div className="min-h-screen bg-gray-50 text-gray-800">
{/* Hero Section */}
<section className="text-center py-16 bg-blue-900 text-white">
<motion.h1 initial={{ opacity: 0, y: -20 }} animate={{ opacity: 1, y: 0 }} className="text-4xl font-bold mb-4">
Trusted Handyman in Toledo – Same-Day Repairs, Done Right.
</motion.h1>
<p className="text-lg max-w-2xl mx-auto">
The Glass City Fixer is your local, reliable handyman service for Toledo and surrounding areas. Fast, honest, and affordable home repairs.
</p>
<a href="#contact" className="inline-block mt-6 px-6 py-3 bg-yellow-400 text-blue-900 font-semibold rounded-lg shadow-md hover:bg-yellow-300 transition">
Get a Free Estimate
</a>
</section>


{/* Services Section */}
<section className="py-16 px-6 max-w-5xl mx-auto" id="services">
<h2 className="text-3xl font-bold text-center mb-10">Our Top Services</h2>
<div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
{['Drywall Repair', 'TV Mounting', 'Light Fixtures', 'Furniture Assembly', 'Minor Plumbing', 'Door & Trim Repair'].map((service) => (
<div key={service} className="bg-white rounded-2xl p-6 shadow-md hover:shadow-xl transition">
<h3 className="font-semibold text-xl mb-2">{service}</h3>
<p className="text-gray-600 text-sm">Professional {service.toLowerCase()} for your home or rental property. Done right, the first time.</p>
</div>
))}
</div>
</section>


{/* About Section */}
<section className="bg-white py-16 px-6" id="about">
<div className="max-w-4xl mx-auto text-center">
<h2 className="text-3xl font-bold mb-4">About The Glass City Fixer</h2>
<p className="text-gray-700 text-lg leading-relaxed">
Hi, I’m Bailey — a local family man born and raised right here in Toledo. I started The Glass City Fixer to provide honest, same-day handyman services that people can actually count on. Whether you need a quick repair or regular maintenance, I treat every job like it’s my own home.
</p>
</div>
</section>


{/* Contact Section */}
<section className="bg-blue-50 py-16 px-6" id="contact">
<div className="max-w-3xl mx-auto text-center">
<h2 className="text-3xl font-bold mb-6">Request a Free Quote</h2>
<p className="text-gray-700 mb-8">Fill out your info below and we’ll reach out to schedule your repair or estimate.</p>


<form onSubmit={handleSubmit} className="grid grid-cols-1 md:grid-cols-2 gap-6 bg-white p-8 rounded-2xl shadow-md">
<input name="name" placeholder="Full Name" onChange={handleChange} value={formData.name} required className="p-3 border rounded-lg" />
<input name="phone" placeholder="Phone Number" onChange={handleChange} value={formData.phone} required className="p-3 border rounded-lg" />
<input name="address" placeholder="Address" onChange={handleChange} value={formData.address} required className="p-3 border rounded-lg md:col-span-2" />
<textarea name="service" placeholder="Type of Service Needed (e.g., drywall, TV mount, plumbing)" onChange={handleChange} value={formData.service} required className="p-3 border rounded-lg md:col-span-2"></textarea>
<button type="submit" className="col-span-2 py-3 bg-blue-900 text-white rounded-lg font-semibold hover:bg-blue-800 transition">Submit Request</button>
</form>
</div>
</section>


{/* Footer */}
<footer className="bg-blue-900 text-white text-center py-6">
<p>© {new Date().getFullYear()} The Glass City Fixer | Toledo, OH</p>
<p className="text-sm mt-1">Handyman | Home Repair | Property Maintenance</p>
</footer>
</div>
);
}
