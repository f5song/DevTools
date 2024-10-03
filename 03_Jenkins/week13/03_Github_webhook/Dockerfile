# ใช้ base image ของ Python 3.9
FROM python:3.9

# ตั้ง working directory ใน container
WORKDIR /code

# คัดลอกไฟล์ requirements.txt และ main.py ไปยัง working directory
COPY requirements.txt ./
COPY main.py ./

# ติดตั้ง dependencies
RUN pip install --no-cache-dir -r requirements.txt

# คำสั่งในการรันแอปพลิเคชัน
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]
