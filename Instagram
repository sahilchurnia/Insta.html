import React from "react";
import { motion } from "framer-motion";

const posts = [
  {
    id: 1,
    username: "@sunnyshots",
    imageUrl: "https://images.unsplash.com/photo-1607746882042-944635dfe10e",
    caption: "Chasing light through the lens.",
    likes: 120,
  },
  {
    id: 2,
    username: "@urbanframes",
    imageUrl: "https://images.unsplash.com/photo-1526170375885-4d8ecf77b99f",
    caption: "City vibes on film.",
    likes: 342,
  },
  {
    id: 3,
    username: "@wildwanderer",
    imageUrl: "https://images.unsplash.com/photo-1500530855697-b586d89ba3ee",
    caption: "Roaming where the wild things are.",
    likes: 225,
  },
];

export default function InstagramClone() {
  return (
    <div className="min-h-screen bg-gray-100 font-sans">
      {/* Header */}
      <header className="flex justify-between items-center px-6 py-4 bg-white shadow-sm sticky top-0 z-10">
        <h1 className="text-2xl font-bold text-pink-500">InstaSnap</h1>
        <input
          type="text"
          placeholder="Search"
          className="border px-3 py-1 rounded-md text-sm focus:outline-none"
        />
        <div className="w-8 h-8 bg-gray-300 rounded-full" />
      </header>

      {/* Feed */}
      <main className="p-4 max-w-2xl mx-auto space-y-6">
        {posts.map((post) => (
          <motion.div
            key={post.id}
            className="bg-white rounded-xl shadow"
            whileHover={{ scale: 1.01 }}
          >
            <div className="flex items-center px-4 pt-4">
              <div className="w-10 h-10 bg-gray-300 rounded-full mr-3" />
              <span className="font-semibold">{post.username}</span>
            </div>
            <img
              src={post.imageUrl}
              alt="Post"
              className="w-full h-96 object-cover mt-2"
            />
            <div className="px-4 py-3">
              <p className="font-semibold">{post.likes} likes</p>
              <p>
                <span className="font-semibold">{post.username}</span> {post.caption}
              </p>
              <button className="text-blue-500 mt-2">Like</button>
            </div>
          </motion.div>
        ))}
      </main>
    </div>
  );
}
