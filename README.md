sparkle.style.left = `${x}px`;
            sparkle.style.top = `${y}px`;
            
            // Random size
            const size = Math.random() * 8 + 3;
            sparkle.style.width = `${size}px`;
            sparkle.style.height = `${size}px`;
            
            // Random opacity
            sparkle.style.opacity = Math.random() * 0.8 + 0.2;
            
            document.body.appendChild(sparkle);
            animateSparkle(sparkle);
        }
        
        // Start the sparkle effect
        createSparkles();
        
        // Continue creating sparkles
        setInterval(createNewSparkle, 500);
        
        // Try to play audio automatically
        document.addEventListener('DOMContentLoaded', function() {
            const audio = document.querySelector('audio');
            if (audio) {
                // Some browsers require user interaction for autoplay
                audio.play().catch(e => {
                    console.log('Autoplay prevented:', e);
                    // Show message to user
                    const audioContainer = document.querySelector('.audio-container');
                    const message = document.createElement('div');
                    message.style.color = '#d32f2f';
                    message.style.fontSize = '0.9rem';
                    message.style.marginTop = '10px';
                    message.innerHTML = '⚠️ Если аудио не воспроизводится, нажмите кнопку воспроизведения';
                    audioContainer.appendChild(message);
                });
            }
        });
    </script>
</body>
</html>
