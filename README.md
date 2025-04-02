import { useState } from "react"; import { Button } from "@/components/ui/button";

export default function App() { const [message, setMessage] = useState("Hello, World!");

const toggleMessage = () => { setMessage((prev) => (prev === "Hello, World!" ? "Welcome to React!" : "Hello, World!")); };

return ( <div className="flex flex-col items-center justify-center min-h-screen bg-gray-100 p-4"> <h1 className="text-2xl font-bold mb-4">React Frontend</h1> <p className="mb-4 text-lg">{message}</p> <Button onClick={toggleMessage} className="px-4 py-2 bg-blue-500 text-white rounded-lg shadow"> Toggle Message </Button> </div> ); }

