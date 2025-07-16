# Autoservicio-Tombri
import React from 'react';

// Main App component for the mobile-optimized offers flyer
const App = () => {
    // Define the offer data, structured by categories with actual image URLs
    const offerData = [
        {
            category: 'Carnes',
            items: [
                { name: 'Punta de espalda el kg', price: '$8990', imageUrl: 'https://placehold.co/100x100/6b21a8/ffffff?text=Punta+Espalda' }, // Placeholder
                { name: 'Pollo fresco el kg', price: '$3890', imageUrl: typeof __file_content_fetcher_url__ !== 'undefined' ? `${__file_content_fetcher_url__}/uploaded:image.png-d7aba79d-9264-46fa-9e7b-20aef9c02457` : 'https://placehold.co/100x100/facc15/ffffff?text=Pollo+Fresco' }, // Image for Pollo fresco
                { name: 'Milanesas de carne el kg', price: '$7990', imageUrl: typeof __file_content_fetcher_url__ !== 'undefined' ? `${__file_content_fetcher_url__}/uploaded:image.png-bf261f06-d3f8-4193-b973-a4e50e43ff65` : 'https://placehold.co/100x100/ef4444/ffffff?text=Milanesa+Carne' }, // Image for Milanesas
                { name: 'Milanesas de cerdo el kg', price: '$5990', imageUrl: typeof __file_content_fetcher_url__ !== 'undefined' ? `${__file_content_fetcher_url__}/uploaded:image.png-bf261f06-d3f8-4193-b973-a4e50e43ff65` : 'https://placehold.co/100x100/ef4444/ffffff?text=Milanesa+Cerdo' }, // Using Milanesas image
                { name: 'Milanesas de pollo el kg', price: '$6990', imageUrl: typeof __file_content_fetcher_url__ !== 'undefined' ? `${__file_content_fetcher_url__}/uploaded:image.png-bf261f06-d3f8-4193-b973-a4e50e43ff65` : 'https://placehold.co/100x100/ef4444/ffffff?text=Milanesa+Pollo' }, // Using Milanesas image
                { name: 'Osobuco el kg', price: '$6200', imageUrl: 'https://placehold.co/100x100/6b21a8/ffffff?text=Osobuco' }, // Placeholder
                { name: 'Carne molida el kg', price: '$6990', imageUrl: typeof __file_content_fetcher_url__ !== 'undefined' ? `${__file_content_fetcher_url__}/uploaded:image.png-7b628978-c07c-4cf6-891c-f03055b386bf` : 'https://placehold.co/100x100/6b21a8/ffffff?text=Carne+Molida' }, // Image for Carne molida
            ],
        },
        {
            category: 'Dulces / Lácteos / Almacén',
            items: [
                { name: 'Dulce de leche x400g', price: '$1598', imageUrl: 'https://placehold.co/100x100/fbbf24/ffffff?text=Dulce+Leche' },
                { name: 'Servilletas Sol Mayor x3 rollos', price: '$1050', imageUrl: 'https://placehold.co/100x100/9ca3af/ffffff?text=Servilletas' },
                { name: 'Masitas Manolio x3 paquetes', price: '$899', imageUrl: 'https://placehold.co/100x100/f97316/ffffff?text=Masitas' },
                { name: 'Shampoo Suave y Acondicionador', price: '$2690', imageUrl: 'https://placehold.co/100x100/38bdf8/ffffff?text=Shampoo' },
                { name: 'Durazno natural x800g', price: '$1339', imageUrl: 'https://placehold.co/100x100/f97316/ffffff?text=Durazno' },
                { name: 'Aceite Cañuela x1500ml Girasol', price: '$3400', imageUrl: 'https://placehold.co/100x100/fde047/ffffff?text=Aceite' },
                { name: 'Fideos Providencia x500g', price: '$649', imageUrl: 'https://placehold.co/100x100/fca5a5/ffffff?text=Fideos' },
                { name: 'Dulce de membrillo el kg', price: '$2200', imageUrl: 'https://placehold.co/100x100/fbbf24/ffffff?text=Membrillo' },
                { name: 'Leche Nido x800g', price: '$8490', imageUrl: 'https://placehold.co/100x100/bfdbfe/ffffff?text=Leche+Nido' },
                { name: 'Yogur Ilolay el sachet', price: '$1499', imageUrl: 'https://placehold.co/100x100/bfdbfe/ffffff?text=Yogur' },
                { name: 'Leche Armonía en tetra', price: '$1250', imageUrl: 'https://placehold.co/100x100/bfdbfe/ffffff?text=Leche+Tetra' },
                { name: 'Puré Molto de tomate x520g', price: '$549', imageUrl: 'https://placehold.co/100x100/dc2626/ffffff?text=Pure+Tomate' },
                { name: 'Arvejas Molto x340g', price: '$399', imageUrl: 'https://placehold.co/100x100/4ade80/ffffff?text=Arvejas' },
            ],
        },
        {
            category: 'Huevos / Lácteos / Enlatados',
            items: [
                { name: 'Maple de huevo', price: '$6399', imageUrl: 'https://placehold.co/100x100/fde047/ffffff?text=Maple+Huevo' },
                { name: 'Queso blando el kg', price: '$6100', imageUrl: typeof __file_content_fetcher_url__ !== 'undefined' ? `${__file_content_fetcher_url__}/uploaded:image.png-00808472-da12-4d47-af0f-57d48e51c54d` : 'https://placehold.co/100x100/bfdbfe/ffffff?text=Queso+Blando' }, // Image for Queso blando
                { name: 'Picadillo Lanera', price: '$569', imageUrl: 'https://placehold.co/100x100/6b7280/ffffff?text=Picadillo' },
                { name: 'Atún Dique x170g', price: '$1099', imageUrl: 'https://placehold.co/100x100/94a3b8/ffffff?text=Atun' },
            ],
        },
        {
            category: 'Otros',
            items: [
                { name: 'Yerba Chamigo x500g', price: '$1199', imageUrl: 'https://placehold.co/100x100/10b981/ffffff?text=Yerba' },
                { name: 'Arroz Primor x1 kilo', price: '$990', imageUrl: 'https://placehold.co/100x100/fde047/ffffff?text=Arroz' },
            ],
        },
    ];

    return (
        <div className="min-h-screen bg-gradient-to-br from-blue-900 to-indigo-950 flex flex-col items-center p-4 font-inter">
            {/* Main Content Card */}
            <div className="bg-white rounded-3xl shadow-2xl p-6 md:p-8 lg:p-10 w-full max-w-md md:max-w-lg transform transition-all duration-500 ease-in-out border-4 border-white border-opacity-20">
                {/* Header Section */}
                <header className="text-center mb-8 w-full">
                    <h1 className="text-5xl md:text-6xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-pink-500 to-red-600 mb-3 drop-shadow-lg">
                        Ofertas Semanales
                    </h1>
                </header>

                {/* Iterate through categories and their items */}
                {offerData.map((categoryData, catIndex) => (
                    <div key={catIndex} className="mb-8 last:mb-0">
                        <h2 className="text-3xl md:text-4xl font-bold text-indigo-400 mb-6 text-center w-full border-b-2 border-indigo-300 pb-4">
                            {categoryData.category}
                        </h2>
                        <ul className="space-y-6 w-full">
                            {categoryData.items.map((item, itemIndex) => (
                                <li key={itemIndex} className="flex items-center bg-gray-50 p-4 rounded-2xl shadow-lg border border-gray-100 hover:shadow-xl transform hover:-translate-y-1 transition-all duration-300 ease-in-out">
                                    {item.imageUrl && (
                                        <img
                                            src={item.imageUrl}
                                            alt={item.name}
                                            className="w-28 h-28 object-cover rounded-2xl mr-4 flex-shrink-0 border-4 border-blue-200"
                                            onError={(e) => { e.target.onerror = null; e.target.src="https://placehold.co/100x100/cccccc/ffffff?text=Producto"; }} // Fallback image
                                        />
                                    )}
                                    <div className="flex flex-col flex-grow text-left">
                                        <span className="text-xl md:text-2xl text-gray-800 font-semibold mb-1">
                                            {item.name}
                                        </span>
                                        <span className="text-2xl md:text-3xl font-extrabold text-green-600">
                                            {item.price}
                                        </span>
                                    </div>
                                </li>
                            ))}
                        </ul>
                    </div>
                ))}

                {/* Footer with business name and address */}
                <footer className="mt-10 pt-6 border-t-2 border-gray-200 text-center text-gray-600 text-sm">
                    <p>¡Visítanos para más ofertas!</p>
                    <p className="text-indigo-600 font-bold mt-1 text-3xl">Autoservicio Tombri</p>
                    <p className="text-gray-500 text-lg mt-2">Córdoba Norte</p>
                </footer>
            </div>
        </div>
    );
};

export default App;
