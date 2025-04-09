import streamlit as st

st.set_page_config(page_title="مساعد المدرب الذكي", layout="centered")

st.title("مساعد المدرب الذكي")
st.markdown("نظام تحليل أداء اللاعبين في الوقت الفعلي وتقديم توصيات تكتيكية للمدرب.")

# بيانات اللاعبين (مثال)
players = [
    {"name": "أحمد المالكي", "number": 10, "distance": 8.2, "fatigue": 82},
    {"name": "خالد الغامدي", "number": 7, "distance": 5.6, "fatigue": 45},
    {"name": "سعود الشهراني", "number": 4, "distance": 9.0, "fatigue": 88}
]

for player in players:
    st.subheader(f"اللاعب رقم {player['number']} - {player['name']}")
    st.write(f"المسافة المقطوعة: {player['distance']} كم")
    st.write(f"مستوى الإرهاق: {player['fatigue']}%")

    if player["fatigue"] > 80:
        st.error("تحذير: اللاعب مرهق جدًا، يُوصى بالتبديل.")
    elif player["fatigue"] > 60:
        st.warning("تنبيه: مستوى الإرهاق مرتفع.")
    else:
        st.success("الوضع مستقر.")

    st.markdown("---")
